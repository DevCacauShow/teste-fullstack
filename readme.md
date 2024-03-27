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
  - Usar proteção de rotas com validação de permissão

### :bangbang: Back-end
Deve ser desenvolvido uma API em .NET com versões igual ou superior à 6 podendo utilizar
  - Sql como banco de dados
  - EF Core ou Dapper como ORM
  - Gravação de log da aplicação no mongodb
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

# 🐙 Formações avançadas

## Alertas

Alertas são uma extensão Markdown baseada na sintaxe blockquote que você pode usar para enfatizar informações críticas. Eles são exibidos com cores e ícones distintos para indicar a importância do conteúdo.

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.

## Seção recolhida

Você pode recolher temporariamente seções do seu Markdown criando uma seção expandida que o leitor pode optar por expandir. Por exemplo, quando você deseja incluir detalhes técnicos em um comentário do problema que pode não ser relevante ou interessante para todos os leitores, você pode colocar esses detalhes em uma seção recolhida.

Qualquer Markdown dentro do bloco `<details>` estará recolhido até que o leitor clique em para expandir os detalhes.

No bloco `<details>`, use a marca `<summary>` para que os leitores saibam o que está dentro dele. O rótulo aparece à direita de .

<details>

<summary>Tips for collapsed sections</summary>

### You can add a header

You can add text within a collapsed section.

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```

</details>

## Diagramas do Mermaid

O Mermeid é uma ferramenta inspirada em Markdown que transforma texto em diagramas. Por exemplo, o Mermeid pode interpretar gráficos de fluxo, diagramas de sequência, gráficos de pizza e muito mais.

Para criar um diagrama do Mermaid, adicione a sintaxe do Mermaid dentro de um bloco de código isolado com o identificador de linguagem mermaid. 

Por exemplo, você pode criar um fluxograma especificando valores e setas.

Here is a simple flow chart:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

## Mapas

É possível usar a sintaxe GeoJSON ou TopoJSON para criar mapas interativos. Para criar um mapa, adicione GeoJSON ou TopoJSON em um bloco de código protegido com o identificador de sintaxe geojson ou topojson. 

```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "id": 1,
      "properties": {
        "ID": 0
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [
              -90,
              35
            ],
            [
              -90,
              30
            ],
            [
              -85,
              30
            ],
            [
              -85,
              35
            ],
            [
              -90,
              35
            ]
          ]
        ]
      }
    }
  ]
}
```
