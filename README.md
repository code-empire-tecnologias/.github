# Code Empire Tecnologias — padrões da organização

Este repositório centraliza templates e, futuramente, documentações compartilhadas
pelos projetos da organização `code-empire-tecnologias`.

Quando publicado como o repositório especial `code-empire-tecnologias/.github`, o
GitHub usa os arquivos de comunidade daqui como padrão nos repositórios que não
possuem uma configuração própria.

## Estrutura atual

```text
.github/
  ISSUE_TEMPLATE/
    config.yml       # configuração do seletor e reporte privado
    epic.yml         # iniciativa ampla e mensurável
    feature.yml      # nova capacidade de produto
    bug.yml          # defeito ou regressão
    tech.yml         # dívida e melhoria técnica
    security.yml     # hardening e redução planejada de risco
docs/
  README.md          # ponto de entrada para documentação futura
```

Todos os formulários adicionam a issue ao Project
[`Pingo Finance`](https://github.com/orgs/code-empire-tecnologias/projects/1).

## Pré-requisitos para publicar

- Criar o repositório `.github` na organização e publicar a branch padrão `main`.
- Manter habilitadas as Issues nos repositórios consumidores.
- Criar as labels `epic`, `security` e `tech-debt` em cada repositório consumidor;
  `bug` e `enhancement` normalmente já existem. O GitHub ignora labels ausentes.
- Garantir permissão de escrita no Project para quem abrir issues, ou habilitar no
  Project um workflow de auto-add para os repositórios da organização.
- Habilitar o reporte privado de vulnerabilidades nos repositórios aplicáveis.

Um repositório pode sobrescrever estes padrões criando os próprios arquivos em
`.github/ISSUE_TEMPLATE`.

## Convenções

- EPIC descreve resultado, métricas e fronteiras; a execução deve ser decomposta em
  sub-issues.
- Feature descreve valor para o usuário e critérios de aceite verificáveis.
- Bug exige reprodução e evidência sanitizada.
- Melhoria técnica explicita custo atual, risco, migração e comprovação.
- Segurança serve para hardening planejado. Vulnerabilidades ativas, incidentes,
  credenciais e exploits devem usar um canal privado.
