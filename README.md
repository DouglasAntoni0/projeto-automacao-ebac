# Projeto de Automação EBAC - Cypress E2E

![Cypress](https://img.shields.io/badge/Cypress-E2E-17202C?style=for-the-badge&logo=cypress&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-automacao-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Cypress Cloud](https://img.shields.io/badge/Cypress%20Cloud-projectId-17202C?style=for-the-badge&logo=cypress&logoColor=white)
![QA](https://img.shields.io/badge/QA-regressao%20continua-0A66C2?style=for-the-badge)

Projeto de automação end-to-end com Cypress para a EBAC Shop, estruturado para validar fluxos web e registrar uma base de execução que pode evoluir para regressão contínua.

Este repositório representa uma etapa de organização de automação: além de executar testes localmente, ele contém configuração que pode ser conectada ao Cypress Cloud e futuramente a pipelines de CI/CD.

## Objetivo do projeto

O objetivo é criar uma base de automação E2E para a EBAC Shop, com foco em:

- configurar Cypress para uma aplicação alvo;
- executar testes no navegador;
- permitir execução headless;
- documentar setup e comandos;
- manter um projeto rastreável no GitHub;
- preparar caminho para dashboard, relatórios e CI/CD.

## Diferencial deste repositório

O `cypress.config.js` possui `projectId`, indicando preparação para integração com Cypress Cloud. Isso aproxima o projeto de um fluxo mais profissional, no qual execuções podem ser registradas, acompanhadas e analisadas ao longo do tempo.

## Stack

| Tecnologia | Papel |
| --- | --- |
| Cypress | Automação E2E |
| JavaScript | Linguagem dos testes |
| Node.js/npm | Runtime e dependências |
| Cypress Cloud | Potencial rastreabilidade de execuções |
| EBAC Shop | Aplicação alvo |

## O que este projeto demonstra

| Competência | Evidência | Valor técnico |
| --- | --- | --- |
| Automação E2E | Cypress aplicado a uma aplicação web de e-commerce | Valida comportamento integrado |
| Configuração de projeto | `cypress.config.js` com `baseUrl` e `projectId` | Prepara execução local e integração futura |
| Execução local | Comandos para headless e runner | Facilita desenvolvimento e manutenção |
| Base para CI/CD | Estrutura pronta para conexão com pipeline | Caminho para regressão contínua |
| Qualidade prática | Exercício tratado como entrega técnica documentada | Melhora leitura pública do repositório |

## Como executar

Clone o repositório:

```bash
git clone https://github.com/DouglasAntoni0/projeto-automacao-ebac.git
cd projeto-automacao-ebac
```

Instale dependências:

```bash
npm install
```

Rodar no terminal:

```bash
npx cypress run
```

Abrir o Cypress Runner:

```bash
npx cypress open
```

## Estratégia de automação

Este projeto pode ser usado como base para:

- smoke tests de fluxos essenciais;
- regressão web;
- validação de jornadas de e-commerce;
- experimentação com Cypress Cloud;
- evolução para execução em pipeline.

A estratégia ideal é manter cenários pequenos, independentes e orientados a comportamento.

## Maturidade técnica esperada

Uma suíte E2E ganha valor quando deixa de ser apenas uma coleção de scripts e passa a funcionar como mecanismo de confiança. Para isso, cada cenário precisa ter intenção clara: qual risco protege, qual fluxo representa e que tipo de falha ajuda a diagnosticar.

Neste projeto, a presença de `baseUrl` e `projectId` indica uma base preparada para crescer. O próximo nível natural seria combinar execução local, dashboard, relatório e pipeline, criando um ciclo em que falhas ficam rastreáveis e decisões de qualidade deixam de depender de validação manual dispersa.

## Boas práticas recomendadas

- Evitar dependência de ordem entre testes.
- Preferir seletores estáveis.
- Centralizar dados em fixtures quando aplicável.
- Criar custom commands para ações repetidas.
- Registrar evidências em relatórios.
- Separar testes críticos de testes exploratórios.

## Leitura de portfólio

Este repositório mostra organização e direção. Mesmo sendo uma base de automação, ele comunica elementos que recrutadores técnicos e lideranças costumam procurar: domínio de setup, clareza de execução, preocupação com rastreabilidade e entendimento de como uma suíte pode evoluir para regressão contínua.

O valor está na fundação: um projeto simples, bem documentado e preparado para crescer é melhor do que uma automação extensa sem comandos claros, evidência ou estratégia de manutenção.

## Troubleshooting

| Situação | Possível causa | Ação |
| --- | --- | --- |
| Cypress Cloud não registra execução | Chave/record não configurado | Configurar token apropriado antes de usar dashboard |
| Aplicação alvo não responde | Ambiente externo fora do ar | Validar acesso manual à EBAC Shop |
| Testes quebram por seletor | DOM alterado | Revisar estratégia de localização |
| Dependências falham | Node/npm incompatível | Atualizar ambiente local |

## Resultado técnico

Este repositório evidencia uma competência importante para QA Automation: transformar exercício em ativo técnico rastreável. A documentação, a configuração e a execução local facilitam manutenção e evolução para relatórios, pipeline e suítes de regressão mais robustas.

## Competências evidenciadas

- Cypress E2E.
- Configuração com `baseUrl`.
- Preparação para Cypress Cloud.
- Execução local e headless.
- Organização de projeto de automação.
- Pensamento de regressão contínua.

## Possíveis evoluções

- Adicionar GitHub Actions.
- Publicar artifacts de execução.
- Integrar Mochawesome.
- Criar matriz de cenários críticos.
- Separar suites por prioridade.
- Adicionar dados dinâmicos para reduzir colisões.

## Conclusão

Este projeto mostra mais do que execução local de Cypress: ele aponta para uma base de automação evolutiva. Com ajustes de arquitetura, relatórios e CI/CD, pode se tornar uma suíte de regressão web mais completa e rastreável.
