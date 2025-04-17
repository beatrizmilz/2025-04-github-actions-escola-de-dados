## Template de prompt para criar um workflow GitHub Actions

Crie um arquivo de workflow (YAML) para o GitHub Actions que automatize o processo de [.......]. 

O workflow deve incluir os seguintes elementos:

- Nome do workflow: Defina um nome descritivo para o workflow, por exemplo, [... descrever com detalhes!].

- Eventos: o workflow deve ser executado em eventos de:
  - Quando a branch main for atualizada (push para a branch main)
  - Em algum dia/horário específico (schedule): [exemplos: todos os dias às 09h no horário de Brasília; toda segunda-feira às 10h no horário de Brasília; todo dia 1º do mês às 12h no horário de Brasília].
  - Quando o botão na interface do GitHub for acionado (workflow_dispatch).

- Jobs: O workflow deve conter um job, que rode em um ambiente linux (ubuntu-latest), e que execute as seguintes etapas:

  - Checkout: Adicione uma etapa para fazer o checkout do código usando a ação oficial actions/checkout (fixe a versão mais recente, por exemplo, `actions/checkout@v2`).

  - Instalação de Dependências: Crie uma etapa para instalar as dependências do projeto (por exemplo, instalar o Python ou o R com `r-lib/actions/setup-r@v2`).
  
  - Execute a tarefa principal: [Adicione uma etapa para executar o script principal do projeto (por exemplo, `script.py` ou `script.R`).]
  
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

- Caso o workflow utilize R, utilize as actions já preparadas no repositório https://github.com/r-lib/actions.

- Caso o workflow utilize Quarto, utilize as actions já preparadas no repositório https://github.com/quarto-dev/quarto-actions.

- Quando possível, utilize ações já existentes no GitHub Marketplace, e dê preferência para ações de criadores verificados: https://github.com/marketplace?verification=verified_creator&type=actions
