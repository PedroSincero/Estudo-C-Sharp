# A estrutura de um projeto para console
Ao criarmos um projeto de aplicação para console, a estrutura básica é iniciada com dois arquivos e uma pasta. Veja mais sobre cada um a seguir:


``` Program.cs ```


Este é o ponto de partida do seu projeto. Neste arquivo você vai escrever o código em C# que será executado quando seu projeto rodar.

Anota aí 🖊: Arquivos com a extensão `.cs` são automaticamente reconhecidos pelo VSCode como arquivos que contém código `C#`. cs de C Sharp.

## < nomeDoProjeto >.csproj 

O `.csproj` é o arquivo de projeto e a base de configuração para projetos `.NET`. Ele vai ser usado para interpretar todas as suas dependências, além de contar com diversas informações de configuração, tais como:

* conteúdo a ser incluído (quais bibliotecas e dependências de terceiros são utilizadas);
* requisitos da plataforma;
* informações de controle da versão;
* configurações do servidor e muito mais.

Cada projeto `.NET` sempre inclui um arquivo de projeto, com uma extensão de arquivo referente ao tipo de projeto. Por exemplo, ao construirmos um projeto em `C#`, o arquivo tem a extensão `.csproj`. Para um projeto `Visual Basic.NET`, o arquivo é `.vbproj`; já para um de banco de dados é usado `.dbproj`. O nome deste arquivo é o mesmo valor utilizado para criar o projeto no parâmetro `-o`, que em nosso caso foi `HelloWorld`.

## Pasta obj/

Por fim, temos a `pasta obj/`, que vai receber as dependências do projeto após rodar o comando `dotnet restore`. Esse comando é semelhante, em termos de funcionalidade, ao comando `npm install` dentro dos projetos Javascript com NodeJS e NPM.

Talvez você possa ter percebido que essa pasta já havia sido criada, mesmo não sendo executado o comando nenhuma vez. Isso ocorre porque alguns outros comandos já o executam implicitamente, caso seja necessário. São eles:

* dotnet new
* dotnet build
* dotnet build-server
* dotnet run
* dotnet test
* dotnet publish
* dotnet pack

Caso você faça uma atualização nas dependências do projeto, instale uma nova biblioteca ou clone um repositório e execute o comando dotnet restore para garantir que todas as dependências foram devidamente baixadas e atualizadas.