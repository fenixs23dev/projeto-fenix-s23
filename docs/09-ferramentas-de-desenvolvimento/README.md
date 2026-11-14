# Ferramentas de Desenvolvimento — Projeto FÊNIX

## 1. Objetivo

Esta seção documenta as ferramentas, automações e processos auxiliares desenvolvidos para organizar, facilitar e acelerar a pesquisa do Projeto FÊNIX.

O objetivo é construir um ambiente de desenvolvimento e investigação que permita executar testes, registrar resultados, preservar evidências e facilitar a continuidade do trabalho.

## 2. Projetos e ferramentas relacionados

### 2.1 SANNY

Assistente desenvolvido para o Samsung Galaxy S23, utilizando Termux. O objetivo é oferecer recursos locais de assistência e automação.

### 2.2 ATLAS BRIDGE

Camada experimental de comunicação e execução controlada, desenvolvida separadamente dentro do projeto SANNY.

A proposta é permitir uma futura integração entre o assistente Atlas, o SANNY e ferramentas locais, mantendo controle de autorização e auditoria.

### 2.3 Ambiente Termux

Ambiente utilizado no Galaxy S23 para desenvolvimento, execução de scripts, testes, organização de arquivos e manutenção das ferramentas.

## 3. Relação com o Projeto FÊNIX

As ferramentas descritas nesta seção são auxiliares à pesquisa de Windows ARM nativo no Samsung Galaxy S23.

Elas não fazem parte do processo de boot do Windows nem substituem os componentes de hardware, firmware, UEFI, kernel ou drivers.

Sua função é apoiar a organização, automação, documentação e reprodutibilidade das investigações.

## 4. Estado atual

- SANNY: desenvolvimento em andamento.
- ATLAS BRIDGE: prova de conceito local implementada.
- Executor: operações restritas por lista de permissões.
- Autorização: confirmação manual antes da execução.
- Auditoria: registro estruturado das operações.
- Comunicação remota com Atlas: ainda não implementada.
- Fila local de tarefas: próxima etapa planejada.

## 5. Organização da documentação

- `atlas-bridge.md`: arquitetura e implementação do ATLAS BRIDGE.
- `automacao.md`: processos de automação.
- `ambiente-de-desenvolvimento.md`: ambiente e ferramentas utilizadas.
- `testes-e-validacoes.md`: testes executados e resultados.
- `historico-de-desenvolvimento.md`: histórico cronológico das alterações.

## 6. Critério de documentação

Toda funcionalidade relevante deverá registrar:

1. Objetivo.
2. Implementação.
3. Ambiente utilizado.
4. Testes realizados.
5. Resultado observado.
6. Limitações conhecidas.
7. Próximas etapas.

Somente resultados efetivamente testados deverão ser apresentados como concluídos.
