<p align="center">
  <img src="https://raw.githubusercontent.com/integraCAR/.github/main/profile/logomarca-integracar.png" alt="IntegraCAR" width="480"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/IFES-Cachoeiro%20de%20Itapemirim-3a7abf?style=flat-square" />
  <img src="https://img.shields.io/badge/IDAF-Espírito%20Santo-3a7abf?style=flat-square" />
  <img src="https://img.shields.io/badge/FAPES-Fundação%20de%20Amparo-e8789c?style=flat-square" />
  <img src="https://img.shields.io/badge/Vigência-2024--2027-3a7abf?style=flat-square" />
</p>

---

## Sobre o Projeto

O **IntegraCAR** é uma iniciativa multi-institucional voltada ao apoio técnico na análise e gestão dos processos do Cadastro Ambiental Rural (CAR) e Simlam no estado do Espírito Santo.

O projeto integra automação de dados, extração automática de informações de documentos, ferramentas de visualização e interoperabilidade com sistemas governamentais, como E-Docs e Simlam, para otimizar o fluxo de trabalho das equipes técnicas envolvidas no processo de regularização ambiental rural. Também produz dados abertos para pesquisa em sensoriamento remoto, como o dataset IntegraCAR-LULC-10K.

O IntegraCAR é conduzido por meio de uma parceria entre o **Idaf**, o **Ifes** e a **Fapes**, com prazo de execução previsto até **maio de 2027**.

---

## Processo de trabalho

Etapas do projeto que não são repositórios, mas fazem parte do caminho de um
processo de CAR.

| Etapa | Descrição | Números |
|---|---|---|
| [Digitalização de processos físicos](https://github.com/integraCAR/integracar-docs/blob/main/processos/digitalizacao.md) | Processos CAR em papel transformados em PDF | 424 processos digitalizados |
| [Autuação no E-Docs](https://github.com/integraCAR/integracar-docs/blob/main/processos/autuacao.md) | Registro dos processos digitalizados no E-Docs e despacho para o grupo IntegraCAR do campus | cerca de 115 processos autuados |
| [Ações de comunicação](https://github.com/integraCAR/integracar-docs/blob/main/processos/comunicacao.md) | Divulgação do projeto, redes sociais, eventos e materiais | - |

---

## Repositórios

O link de cada nome leva à **documentação** do sistema, no repositório público
[integracar-docs](https://github.com/integraCAR/integracar-docs). A maior parte
do código é privada; a documentação é aberta.

### Gestão de processos

| Repositório | Descrição | Visibilidade | Status |
|---|---|---|---|
| [integracar-gestao](https://github.com/integraCAR/integracar-docs/blob/main/gestao/README.md) | Sistema web onde bolsistas, orientadores e coordenadores enviam os PDFs, revisam campo a campo o que foi extraído e registram atividades | Privado | Ativo |
| [integracar-dashboard](https://github.com/integraCAR/integracar-docs/blob/main/dashboard/README.md) | Painel Streamlit com os processos IntegraCAR consolidados a partir da API do E-Docs | Privado | Ativo |

### Extração automática de documentos

| Repositório | Descrição | Visibilidade | Status |
|---|---|---|---|
| [integracar-backend-extrator](https://github.com/integraCAR/integracar-docs/blob/main/extrator/api.md) | API FastAPI + Postgres: fila, documentos extraídos, histórico de versões e API pública | Privado | Ativo |
| [integracar-ocr-extrator](https://github.com/integraCAR/integracar-docs/blob/main/extrator/worker-ocr.md) | Worker de OCR com GLM-OCR (Ollama) e extração de campos por regex + LLM | Privado | Ativo |
| [integracar-infra-extrator](https://github.com/integraCAR/integracar-docs/blob/main/extrator/infra.md) | Stack Docker da extração, gateway, observabilidade e backup | Privado | Ativo |
| [PDF-Pesquisavel](https://github.com/integraCAR/integracar-docs/blob/main/extrator/pdf-pesquisavel.md) | Gera a camada de texto dos PDFs escaneados (OCRmyPDF) | Privado | Ativo |

### Pesquisa: uso e cobertura do solo

| Repositório | Descrição | Visibilidade | Status |
|---|---|---|---|
| [integracar-lulc-builder](https://github.com/integraCAR/integracar-docs/blob/main/lulc/README.md) | Pipeline que baixa imagens de satélite e mapas de uso do solo do GeoBases ([código](https://github.com/integraCAR/integracar-lulc-builder)) | Público | Ativo |
| [IntegraCAR-LULC-10K](https://github.com/integraCAR/integracar-docs/blob/main/lulc/README.md#integracar-lulc-10k-landing-page) | Página do dataset IntegraCAR-LULC-10K ([código](https://github.com/integraCAR/IntegraCAR-LULC-10K) · [dataset](https://huggingface.co/datasets/laicsiifes/IntegraCAR-LULC-10K)) | Público | Ativo |

### Web e documentação

| Repositório | Descrição | Visibilidade | Status |
|---|---|---|---|
| [integracar-web](https://github.com/integraCAR/integracar-docs/blob/main/web/README.md) | Site institucional do projeto | Público | Planejado |
| [LANDING-PAGE-INTEGRACAR-ES](https://github.com/integraCAR/integracar-docs/blob/main/web/README.md#landing-page-integracar-es) | Versão anterior da página do dataset | Privado | Legado |
| [integracar-docs](https://github.com/integraCAR/integracar-docs) | Documentação técnica, arquitetura e integrações de todos os sistemas | Público | Em construção |
| [.github](https://github.com/integraCAR/.github) | Esta página de apresentação da organização | Público | Ativo |

---

## Instituições Parceiras

| Instituição | Papel |
|---|---|
| IFES - Instituto Federal do Espírito Santo, Campus Cachoeiro de Itapemirim | Desenvolvimento técnico e pesquisa |
| IDAF - Instituto de Defesa Agropecuária e Florestal do ES | Parceiro operacional |
| FAPES - Fundação de Amparo à Pesquisa do ES | Fomento à pesquisa |
| Governo do Estado do Espírito Santo / SEGER | Parceiro institucional |
| Inova IFES | Apoio à inovação |
| SERD | Parceiro |
| CREA | Parceiro |
| CRTES | Parceiro |

---

## Tecnologias

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white" />
  <img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white" />
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
</p>

---

## Equipe Desenvolvedora

- Arthur Gonçalves
- Beatriz Ruela
- Cauã Marvila
- Eduardo Esquincalha
- Gabriela Marques
- Lucas Altoé
- Mikaela Cantalejo
- Murilo Cruz
- Pedro Almeida

---

## Contato

Coordenação de TI: IFES Campus Cachoeiro de Itapemirim
Site do projeto: [integracar.agr.br](https://integracar.agr.br)
