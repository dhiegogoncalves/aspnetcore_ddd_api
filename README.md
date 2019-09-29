# API .NET Core

> Este projeto é uma API desenvolvida com a metodologia DDD, utilizando .NET Core + Entity Framework Core + Swagger + AutoMapper + JWT.

![Capturar](https://user-images.githubusercontent.com/6399309/65838294-aec89780-e2cf-11e9-869b-66075e8bb79e.PNG)

### Iniciar a aplicacão :checkered_flag:

Depois de efetuar o download da aplicação, acesse a pasta `./src/` e execute o comando abaixo para efetuar o download das dependências e efetuar o build da aplicação:

```console
dotnet build
```

A aplicação foi desenvolvida com o banco de dados PostgreSQL. Para alterar a string de conexão acesse o arquivo `./src/Api.Data/Context/ContextFactory.cs` e modifique o retorno da função `ConnectionString`.

Acesse a pasta `./src/Api.Data/` e execute o comando abaixo para configurar o banco de dados:

```console
dotnet ef database update
```

_NOTA: Caso aconteça algum erro no comando `ef`, execute o comando `dotnet tool install --global dotnet-ef --version 3.0.0` para instalar o pacote de comandos do Entity Framework Core e depois execute o comando acima de novo._

Por fim para rodar a aplicação esteja na pasta raiz da aplicação `./` e execute o comando:

```console
dotnet run --project ./src/Api.Application/
```

Para visualizar a aplicação acesse o endereço [http://localhost:5001](http://localhost:5001) no navegador.
