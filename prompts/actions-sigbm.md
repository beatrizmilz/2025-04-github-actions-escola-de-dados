> Este foi o prompt inicial utilizado durante a aula para gerar o arquivo de workflow do GitHub Actions.

Crie um arquivo de workflow (YAML) para o GitHub Actions que automatize o processo de: fazer o download de um arquivo excel (.xlsx) dos dados do sistema SIGBM
o link da API é https://app.anm.gov.br/SIGBM/Publico/ClassificacaoNacionalDaBarragem/ExportarExcel
o método usado pela API é POST
quero que salve o arquivo em uma pasta chamada "data/"
quero que salve uma marcação da data do download no nome do arquivo
quero que faça commit do arquivo baixado para o repositório

O workflow deve incluir os seguintes elementos:

- Nome do workflow: Defina um nome descritivo para o workflow

- Eventos: o workflow deve ser executado em eventos de:
  - Em algum dia/horário específico (schedule): todos os dias às 09h no horário de Brasília.
  - Quando o botão na interface do GitHub for acionado (workflow_dispatch).

- Jobs: O workflow deve conter um job, que rode em um ambiente linux (ubuntu-latest), e que execute as seguintes etapas:

  - Checkout: Adicione uma etapa para fazer o checkout do código usando a ação oficial actions/checkout (fixe a versão mais recente, por exemplo, actions/checkout@v2).

  
  - Execute a tarefa principal: fazer download dos dados
  
  - Faça commit e push dos arquivos gerados: Adicione uma etapa para fazer commit e push dos arquivos gerados ou atualizados pelo script para o repositório. 
  
  - Quando fizer commit, utilize o seguinte nome e email:
  

git config --local user.email "...."
git config --local user.name "...."

  

Siga essas boas práticas:

- Configure o GITHUB_TOKEN com as permissões mínimas necessárias.

- Comentários e Legibilidade: Insira comentários curtos no arquivo explicando a finalidade de cada etapa, facilitando o entendimento para usuários com pouca experiência em GitHub Actions.
        
- O workflow deve seguir as melhores práticas da documentação oficial do GitHub Actions: https://docs.github.com/pt/actions

- Caso o workflow utilize R, utilize as actions já preparadas no repositório https://github.com/r-lib/actions.
