# :memo: Teste técnico Fullstack - CacauShow
Neste repositório você irá encontrar o enunciado do teste técnico para vaga de Fullstack Developer da [CacauShow](https://www.cacaushow.com.br/para-sua-empresa/para-sua-empresa.html)!
Você provavelmente chegou aqui após passar pelas outras etapas do processo seletivo. Se está não for o seu caso e mesmo assim você implementar alguma solução para este exercício ele **não** será avaliado.

> [!NOTE]
> Você pode usar o problema descrito aqui para exercitar suas habilidades de desenvolvimento, mas a sua solução será avaliada por alguém da Cacau Show apenas se você estiver no processo seletivo da vaga.

## :rotating_light: O Desafio
O seu objetivo é criar uma aplicação que seja capaz de gerenciar usuários, portanto, será necessário ter uma tela de login, listagem com paginação, filtros de busca por nome, e-mail e/ou nível e botões de ação para edição e exclusão, criação de tela de cadastro, edição e exclusão (podendo ser um modal), os usuários deve possuir os seguintes campos.
  - Nome (obrigatório): Deve ser informado o nome completo
  - Data Nascimento (obrigatório): Em formato BR (dd-MM-yyyy)
  - E-mail (obrigatório): Incluir validação de formato de e-mail e o mesmo será utilizado posteriormente para login
  - Nível (obrigatório): Podendo ser
    - Admin: Pode se logar, cadastrar, excluir, editar e visualizar usuários
    - Usuário: Pode se logar e visualizar apenas a tela de listagem, deixando os botões de edição e exclusão ocultos
  - Lista de endereço (obrigatório): Podendo ter ao menos um preenchido
    - Ao digitar o CEP, realizar busca no ViaCep ou qualquer outra API de endereço para preenchimento automático dos campos de Cidade, Bairro e Logradouro

### :globe_with_meridians: Front-end
Deve ser desenvolvido uma aplicação em **Angular** com versões igual ou superior à 16x podendo
  - Separar rotas em module, em caso de versão superior a 16, utilizar standalone
  - Gostariamos de avaliar a sua habilidade com Scss e semântica HTML, portanto, **NÃO** utilizar biblioteca para os componentes (Bootstrap, material, ...)
  - Utilizar de Pipe para campos com mascaras ou podendo utilizar biblioteca para máscaras
  - Usar Guard Routes com validação de permissão para os níveis de admin e usuário, em nível de acesso de botão, utilizar diretivas
  - Utilizar de interfaces tipadas
  - Incluir validação de campos
  
### :hash: Back-end
Deve ser desenvolvido uma API em **.NET** com versões igual ou superior à 6 podendo utilizar
  - Além de JWT em endpoints privados (listar, adicionar, atualizar, excluir), incluir x-api-key em todas as requisições
  - Somente nível admin pode acessar os endpoints de criar, editar e excluir, nível usuário só pode listar
  - EF Core ou Dapper como ORM/Micro ORM
  - Gravação de log da aplicação no mongodb com Serilog
  - Incluir cache distribuído com redis apenas no endpoint de GET de usuário 
  - Gostariamos de avaliar o seu nível de arquitetura, portanto, fazer separação em camadas seguindo o padrão do DDD
  - Don't repeat yourself, portanto, utilize classe blases para não repetição de código
  - Sql como banco de dados
  - Gerar script SQL para criação de tabelas

### :page_facing_up: Regras de negócio
  - Não permitir cadastrar usuário com mesmo E-mail
  - Não permitir nomes com mais de 100 caracteres
  - Não permitir cadastro para menores de 18 anos
  - Não permitir a inclusão de endereços iguais

### :heavy_plus_sign: Plus 
- Instruções no readme
- Qualidade de código
- Cross browser and device (mobile, tablet e desktop)
- Testes
- Resete de senha
- Utilizar dockerfile e dockercompose

> [!IMPORTANT]
> Após finalizar o projeto, criar um repositório no github e dar acesso para o e-mail desenvolvimento@cacaushow.com.br

### :four_leaf_clover: Boa sorte
<!-- 
> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions. -->
