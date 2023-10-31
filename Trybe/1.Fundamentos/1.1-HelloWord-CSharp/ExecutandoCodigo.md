# Executando código C#
O .NET fornece um jeito rápido e prático para compilar código utilizando a CLI. De dentro da pasta de um projeto execute:
```
dotnet build
```
Esse comando vai gerar um programa executável de seu projeto e armazenar na pasta bin/

E agora, para executar esse código, basta rodar o comando:
```
dotnet run
```
Esse comando vai executar a aplicação no mesmo terminal em que você executou o comando dotnet run. E caso a sua aplicação seja a mesma do modelo para console criada com dotnet new console