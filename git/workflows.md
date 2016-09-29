# Git workflows

Os workflows são, traduzindo literalmente do inglês, fluxos de trabalho. No Git, existem 4 principais fluxos de trabalho: o **Centralized Workflow**, o **Feature Branch Workflow**, o **Gitflow Workflow** e o **Forking Workflow**.

Cada workflow funciona de uma maneira e o objetivo deste artigo é explicar resumidamente seu funcionamento, além de citar algumas vantagens e desvantagens de cada fluxo.

## Centralized

O *Centralized Workflow* traz o funcionamento básico do Git, pull, commit, merge, rebase e push. Nesse fluxo, todos os integrantes do time trabalham em cima da mesma versão do código, ou seja, no mesmo repositório e na mesma branch, daí o nome "Centralized", pois todo o desenvolvimento fica centralizado em uma única branch em um único repositório.

Nesse workflow, os membros fazem uma cópia local do repositório (_clone_) e já podem começar a trabalhar no código.

### Vantagens e desvantagens

**Vantagens**

- Qualquer um com conhecimentos básicos de versionamento pode começar a trabalhar no projeto sem maiores dificuldades

- Equipes pequenas se habituarão muito fácil à ferramenta

**Desvantagens**

 - Fica difícil de ter controle sobre as releases do código, uma vez que todos vão trabalhando e comitando suas versões umas atrás das outras

 - Para equipes muito grandes podem ter problemas com merges

## Feature Branch

 ...
