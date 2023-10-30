# Preparando nosso computador para o desenvolvimento com .NET
Nativamente, o .NET é utilizado no sistema operacional Windows, no entanto, com a criação do framework .NET Core, se tornou possível o uso em ambiente Linux, o qual será utilizado para o desenvolvimento das aplicações.

# Instalando o .NET Core no linux
Antes de instalar o Software Development Kit (SDK) da plataforma de desenvolvimento, precisamos garantir que não há nenhuma versão do .NET já instalada, então remova qualquer versão já existente com o comando:

```bash
sudo apt-get remove 'dotnet*'
```
Agora, só para confirmar que removemos com sucesso, use o comando:

```bash
apt list --installed "dotnet*"
```

Primeiro atualize os repositórios no Ubuntu:

```bash
sudo apt-get update
```
Agora vamos instalar o runtime do .NET com o comando:

```bash
sudo apt install aspnetcore-runtime-6.0
```
Após a instalação do runtime, execute este comando para validar os pacotes .net instalados.:
 ```bash
 apt list --installed "dotnet*"
 ```

Após vamos instalar a SDK do .NET, é ele que permite o desenvolvimento dos aplicativos na plataforma do .NET. Para sua instalação, use o comando abaixo:

```bash
sudo apt install dotnet6
```
Pronto! 🎉 Agora, para testar se o .NET Core foi instalado com sucesso, execute o comando:

```bash
$ dotnet --info
```
