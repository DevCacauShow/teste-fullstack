# :memo: Teste técnico Fullstack - CacauShow
Neste repositório você irá encontrar o enunciado do teste técnico para vaga de Fullstack Developer da [CacauShow](https://www.cacaushow.com.br/para-sua-empresa/para-sua-empresa.html)!
Você provavelmente chegou aqui após passar pelas outras etapas do processo seletivo. Se está não for o seu caso e mesmo assim você implementar alguma solução para este exercício ele **não** será avaliado.

> [!NOTE]
> Você pode usar o problema descrito aqui para exercitar suas habilidades de desenvolvimento, mas a sua solução será avaliada por alguém da Cacau Show apenas se você estiver no processo seletivo da vaga.

## :heavy_exclamation_mark: O Desafio
O seu objetivo é criar uma aplicação que seja capaz de gerenciar usuários, portanto, será necessário ter uma tela de login, listagem com paginação e filtros de busca, cadastro, edição e exclusão, os usuários deve possuir os seguintes campos.
  - Nome (obrigatório): Deve ser informado o nome completo
  - Data Nascimento (obrigatório): Em formato BR (dd-MM-yyyy)
  - E-mail (obrigatório): Incluir validação de formato de e-mail
  - Nível (obrigatório): Podendo ser
    - Admin: Pode se logar, cadastrar, excluir, editar e visualizar usuários
    - Usuário: Pode se logar e visualizar apenas a tela de listagem

### :bangbang: Front-end
Deve ser desenvolvido uma aplicação em **Angular** com versões igual ou superior à 16x podendo
  - Separar as rotas em module
  - Gostariamos de avaliar a sua habilidade com SCSS e semântica HTML, portanto, não utilizar biblioteca para os componentes
  - Utilizar de Pipe para campos com mascaras
  - Usar Guard Routes com validação de permissão
  - Em caso de versão acima do 16 utilizar standalone igual a true

### :bangbang: Back-end
Deve ser desenvolvido uma API em .NET com versões igual ou superior à 6 podendo utilizar
  - Sql como banco de dados
  - EF Core ou Dapper como ORM
  - Gravação de log da aplicação no mongodb com Serilog
  - Uso do redis em GET de usuário

### :page_facing_up: Regras de negócio
  - Não permitir um usuário com mesmo E-mail
  - Não permitir nomes com mais de 100 caracteres
  - Não permitir cadastro para menores de 18 anos

### :heavy_plus_sign: Plus
- Instruções no readme
- Utilizar dockerfile e dockercompose
- Qualidade de código
- Cross browser and device (mobile, tablet e desktop)
- Testes

> [!IMPORTANT]
> Após finalizar o projeto, criar um repositório no github e dar acesso para o e-mail desenvolvimento@cacaushow.com.br

## Boa sorte!
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
