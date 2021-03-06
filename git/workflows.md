# Git workflows

Os workflows são, traduzindo literalmente do inglês, fluxos de trabalho. No Git, existem 4 principais fluxos de trabalho: o **[Centralized Workflow](#centralized)**, o **[Feature Branch Workflow](#feature-branch)**, o **[Gitflow Workflow](#gitflow)** e o **[Forking Workflow](#forking)**.

Cada workflow funciona de uma maneira e o objetivo deste artigo é explicar resumidamente seu funcionamento, além de citar algumas vantagens e desvantagens de cada fluxo.

## Centralized

O _Centralized Workflow_ traz o funcionamento básico do Git: _pull_, _commit_, _merge_ e _push_. Nesse fluxo, todos os integrantes do time trabalham em cima da mesma versão do código, ou seja, no mesmo repositório e na mesma branch, daí o nome "Centralized", pois todo o desenvolvimento fica centralizado em uma única branch em um único repositório.

Nesse workflow, os membros fazem uma cópia local do repositório (_clone_) e já podem começar a trabalhar no código. Depois que as alterações foram feitas, segue-se o seguinte fluxo:

1. commit das alterações;
2. pull para sincronizar com a versão do servidor;
3. merge (se necessário);
4. finalmente o push para enviar a versão atualizada e mesclada ("_mergeada_").


**Vantagens**

- Qualquer um com conhecimentos básicos de versionamento pode começar a trabalhar no projeto sem maiores dificuldades

- Equipes pequenas se habituarão muito fácil à ferramenta

**Desvantagens**

 - Fica difícil de ter controle sobre as releases do código, uma vez que todos vão trabalhando e comitando suas versões umas atrás das outras

 - Equipes muito grandes podem ter problemas com merges

## Feature Branch

O _Feature Branch Workflow_ adiciona ao workflow anterior a opção de separar o desenvolvimento em branches, sendo uma branch para cada nova feature no site.

Geralmente as branches são nomeadas com o nome resumido da feature _(ex: novo-menu-logado)_ ou, se esse branch for dedicado à uma correção de bug, com um identificador e o numero _(ex: bug-1661)_.

**Vantagens**

- Melhora o merge
- As versões ficam mais fáceis de serem encontradas
- Mantém separado da master features que possam quebrar o sistema
- Permite a utilização de pull requests na master
- mantem o código da master sempre em conformidade com o que é publicado

**Desvantagens**

- times muito grandes atuando em sistemas muito grandes podem acabar se perdendo com a infinidade de branches que serão criados

## Gitflow
