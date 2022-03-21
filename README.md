Para iniciar uma nova classlib:
```bash
dotnet new classlib -n Play.Common --framework net5.0
```

Adicionar os pacotes:
```bash
dotnet add package MongoDB.Driver
dotnet add package Microsoft.Extensions.Configuration
dotnet add package Microsoft.Extensions.Configuration.Binder
dotnet add package Microsoft.Extensions.DependencyInjection
```

É necessário realizar o empacotamento do serviço para ser usado em outros serviços, para isso é necessário indicar o caminho onde o pacote ficará, criando um pacote nuget. No meu caso é:
```bash
dotnet pack -o ../../../packages/
``` 
