Crie um arquivo de workflow (YAML) para o GitHub Actions que automatize o processo de fazer o download de um arquivo excel com os dados diários do SIGBM, e salvar no repositório. O nome do arquivo deve conter uma timestamp com o dia em que foi executado. O arquivo está em: https://app.anm.gov.br/SIGBM/Publico/ClassificacaoNacionalDaBarragem/ExportarExcel . Os arquivos devem ser salvos na pasta "data". O método de download deve ser POST.

O workflow deve incluir os seguintes elementos:

- Nome do workflow: Defina um nome descritivo para o workflow, por exemplo, "download-sigbm".

- Eventos: o workflow deve ser executado em eventos de:
  - Em algum dia/horário específico (schedule): [todos os dias às 08h no horário de Brasília].
  - Quando o botão na interface do GitHub for acionado (workflow_dispatch).

- Jobs: O workflow deve conter um job, que rode em um ambiente linux (ubuntu-latest), e que execute as seguintes etapas:

  - Checkout: Adicione uma etapa para fazer o checkout do código usando a ação oficial actions/checkout (fixe a versão mais recente, por exemplo, actions/checkout@v2).

  - Execute tarefa principal: a etapa de download dos dados usando a linha de comando.
  
  - Faça commit e push dos arquivos gerados: Adicione uma etapa para fazer commit e push dos arquivos gerados ou atualizados pelo script para o repositório. 
  
  - Quando fizer commit, utilize o seguinte nome e email:
  
```
git config --local user.email "...."
git config --local user.name "...."
```  

Siga essas boas práticas:

- Configure o GITHUB_TOKEN com as permissões mínimas necessárias.

- Comentários e Legibilidade: Insira comentários curtos no arquivo explicando a finalidade de cada etapa, facilitando o entendimento para usuários com pouca experiência em GitHub Actions.
        
- O workflow deve seguir as melhores práticas da documentação oficial do GitHub Actions: https://docs.github.com/pt/actions
