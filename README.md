# Battle Royalle Service

Aplicação cliente que executa como um Windows Service, aplicação Web para prover a interface que permite executar os comandos em uma ou várias máquinas.
Com a aplicação Web é possível escolher uma máquina para interagir com ela executando comandos e recebendo os resultados dele, ou seja, um terminal na aplicação web.

## Começando

O projeto é dividido em três partes: Windows Console Application, ASP.NET Core with Vue.js e ASP.NET Core Web API.

### Pré-requisitos

Para desenvolvimento e execução de testes a devem ser instalados na máquina:

```
.NET Core 2.2 ou superior
Node.js
Visual Studio Code (recomandável para Windows, Linux e Mac)
Visual Studio 2017 ou superior (opcional no Windows ou Mac)
```

### Instalação

Deve ser criado uma Blank Solution no Visual Studio com o nome BattleRoyalle, ou executar o no prompt do Windows ou terminal (Linux e Mac) os seguintes comandos:

```
dotnet new sln -o BattleRoyalle
```

Dentro do diretório BattleRoyalle devem ser executados os seguintes comandos para serem criados os projetos:

```
dotnet new webapi -o BattleRoyalle.API
dotnet new console -o BattleRoyalle.Service
dotnet new nunit -o BattleRoyalle.Tests
dotnet new vue -o BattleRoyalle.WebUI
```

Caso algum dos comandos acima não funcione no terminal, o seguinte comando deve ser executado para habilitá-los:

```
dotnet new --install Microsoft.AspNetCore.SpaTemplates::*
```

Com os projetos criados no diretório BattleRoyalle, devem ser ecxecutados os seguintes comandos para adicionar os mesmos à solução:

```
dotnet sln BattleRoyalle.sln add BattleRoyalle.API/BattleRoyalle.API.csproj
dotnet sln BattleRoyalle.sln add BattleRoyalle.Service/BattleRoyalle.Service.csproj
dotnet sln BattleRoyalle.sln add BattleRoyalle.Tests/BattleRoyalle.Tests.csproj
dotnet sln BattleRoyalle.sln add BattleRoyalle.WebUI/BattleRoyalle.WebUI.csproj
```

## Executando os testes

Explicar como executar os testes automatizados para este sistema.

### Divida em testes de ponta a ponta

Explique o que esses testes testam e por quê.

```
Dê um exemplo.
```

## Publicação

Adicione notas adicionais sobre como implantar isso em um sistema.

## Construído com

* [.NET Core](https://dotnet.microsoft.com/download/) - Framework gratuito, de código aberto desenvolvido pela Microsoft e pela comunidade.
* [Vue.js](https://vuejs.org/) - Estrutura JavaScript de código aberto para criar interfaces com o usuário e aplicativos de página única (SPA).
* [Node.js](https://nodejs.org/) - Interpretador de código JavaScript com o código aberto, focado em migrar o Javascript do lado do cliente para servidores.

## Autores

* **Stanislaw Cruz** - *Trabalho inicial* - [stanycruz](https://github.com/stanycruz)
* **Francisco Wallison** - *Front-end* - [FranciscoWallison](https://github.com/FranciscoWallison)
* **Maria Eduarda Amaral** - *Front-end e back-end* - [MariaAmaralSB](https://github.com/MariaAmaralSB)

Veja também a lista de [colaboradores](https://github.com/desafiando-dev-s/BattleRoyalle/graphs/contributors) que participaram deste projeto.

## Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE.md](LICENSE.md) para detalhes.

## Agradecimentos

* Comente sobre o código que foi utilizado.
* Inspiração.
* etc.
