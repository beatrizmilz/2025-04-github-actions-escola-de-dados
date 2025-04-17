# Automatize tarefas com GitHub Actions:  Primeiros passos

Materiais utilizados no webinar "Automatize tarefas com GitHub Actions: Primeiros passos", apresentado por [Beatriz Milz](https://beamilz.com), e organizado pela [Escola de Dados](https://escoladedados.org).

## Materiais

- Slides: [Canva](https://www.canva.com/design/DAGkzIv8-og/f_HNMAF6MYzA6Bcs_-Kirg/edit?utm_content=DAGkzIv8-og&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton) e [PDF](https://github.com/beatrizmilz/2025-04-github-actions-escola-de-dados/tree/main/slides.pdf)

- [Scripts](https://github.com/beatrizmilz/2025-04-github-actions-escola-de-dados/tree/main/.github/workflows)

- [Prompts](https://github.com/beatrizmilz/2025-04-github-actions-escola-de-dados/tree/main/prompts)

## Materiais extras

### Git e GitHub

- [Tutorial Introdução ao Git e GitHub: colaborando com projetos de código aberto](https://escoladedados.org/tutoriais/introducao-ao-git-e-github-colaborando-com-projetos-de-codigo-aberto/), escrito por Anicely Santos,
  e publicado na Escola de Dados.

- [Material da aula "introdução ao controle de versão com Git e GitHub"](https://ipeadata-lab.github.io/curso_r_intermediario_202501/git-github.html) ministrado por Beatriz Milz no curso de R Intermediário da IPEA.

- [Curso gratuito: Git e GitHub ](https://cursos.teomewhy.org/material_2025), ministrado pelo Teo Calvo (teomewhy).


### GitHub Actions

- [Documentação do GitHub Actions](https://docs.github.com/pt/actions)

- [GitHub Actions for the R language](https://github.com/r-lib/actions), para quem usa R.

- [GitHub Actions for Quarto](https://github.com/quarto-dev/quarto-actions)

- [GitHub Actions Marketplace](https://github.com/marketplace?verification=verified_creator&type=actions)

### Outros

- [Webinar Escola de Dados: Como descobrir APIs escondidas para facilitar a raspagem de dados](https://escoladedados.org/webinar/como-descobrir-apis-escondidas-para-facilitar-a-raspagem-de-dados/)

- [crontab guru - ferramenta para criar o texto para  do `schedule`](https://crontab.guru/)

## Exemplos de projetos que usam GitHub Actions

- [Bash] [`beatrizmilz/sigbm`- Download das tabelas do SIGBM](https://github.com/beatrizmilz/sigbm/blob/main/.github/workflows/download-sigbm.yaml)

- [Python] [`jtrecenti/goal500-python` - raspa informações da Wikipedia sobre gols por jogadores de futebol](https://github.com/jtrecenti/goal500-python)


- [R] [`beatrizmilz/iptgrh_scraper`- Faz download de páginas HTML](https://github.com/beatrizmilz/iptgrh_scraper/blob/master/.github/workflows/executar-script-download-html.yaml)

- [R + Quarto] [`ipeadata-lab/curso_r_intro_202409` - Renderiza o livro em Quarto sempre que o repositório é atualizado](https://github.com/ipeadata-lab/curso_r_intro_202409/blob/main/.github/workflows/quarto-render.yaml)


Alguns que estão quebrados, e preciso arrumar:

- [R] [`beatrizmilz/mananciais` -Faz download dos dados do portal de Mananciais da Sabesp](https://github.com/beatrizmilz/mananciais/blob/master/.github/workflows/2-update_data.yaml)

- [R] [`beatrizmilz/scieloPeriodicos` - Raspa a lista de periódicos científicos da coleção Scielo e suas páginas de instruções](https://github.com/beatrizmilz/scieloPeriodicos/tree/main/.github/workflows)

- [R] [`jtrecenti/goal500` - raspa informações da Wikipedia sobre gols por jogadores de futebol](https://github.com/jtrecenti/goal500)


### Materiais anteriores (elaborados por Beatriz Milz)

- Apresentações:
  - [Utilizando GitHub Actions para baixar dados públicos - Um exemplo com dados de barragens de mineração](https://beamilz.com/talks/pt/2023-04-cervejacomdados-fortaleza/)
  - [Running code while we’re sleeping - Introduction to GitHub Actions for R users](https://beamilz.com/talks/en/2022-gha-rladies-abuja/)
  - [Making awesome automations with GitHub Actions - rstudio::conf(2022)](https://beamilz.com/talks/en/2022-rstudio-conf/)
  - [Introdução ao GitHub Actions](https://beamilz.com/talks/pt/2021-github-actions-gyn/)
  - [Coleta de dados automatizada e integração contínua utilizando GitHub Actions](https://beamilz.com/talks/pt/2021-ser-uff/)


- Posts:
  - [Introdução ao GitHub Actions para quem programa em R](https://beamilz.com/posts/series-gha/2022-series-gha-1-what-is/pt/)
  - [Monitoring quarto-dev repositories: Creating a workflow with GitHub Actions for R users](https://beamilz.com/posts/series-gha/2022-series-gha-2-creating-your-first-action/en/)
  - [How important is GitHub Actions to RStudio/Posit?](https://beamilz.com/posts/series-gha/2022-07-28-github-actions-rstudio/en/)
  


## Ferramentas utilizadas na apresentação

- [carbon](https://carbon.now.sh/) para gerar imagens de código

- [canva](https://www.canva.com/) para criar a apresentação

- [chatGPT](https://chat.openai.com/) para fazer algumas demonstrações
