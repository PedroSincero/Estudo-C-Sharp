# Criando projetos .NET com a CLI

Ao criar um novo projeto de aplicação para console, o comando a ser utilizado é:

```
dotnet new console
```

Esse comando vai criar um projeto .NET utilizando como base um modelo pré-configurado para aplicações de console.

```
dotnet new --help
```
Outra possibilidade é ver as opções disponíveis para o modelo específico que estiver criando, no nosso caso, o console com:
```
dotnet new console --help
 ```
Uma das opções disponíveis é a de já direcionar a saída desse comando para uma pasta específica com a option ```-o```. É super prático para já separar novos projetos em pastas diferentes, e ainda quando usamos isso o projeto já fica nomeado com o nome que passamos para essa option. Vamos ver adiante nessa lição mais detalhes sobre essa nomeação de projetos criados.
```
dotnet new console -o <nome da pasta>
```

Agora que você já sabe sobre a funcionalidade do comando dotnet new console , vamos usá-lo na criação de uma nova aplicação.

Em seu terminal, execute o seguinte comando:

```
dotnet new console -o HelloWorld
```
Quando a execução finalizar, você vai perceber que uma nova pasta chamada HelloWorld foi criada. Para acessá-la, utilize o comando ```cd HelloWorld/```.
