# SIGOS - Gestão de Ordens de Serviço

O projeto tem como objetivo o gerenciamento de um sistema de Ordens de Serviço, por meio de controle e acesso a dados relacionados ás ordens de serviços, usuários, clientes e serviços de maneira acessível e intuitiva.

**Colaboradores:** 
Arthur Araujo Lima| Roberta Maria Lansana

## Tecnologias Utilizadas
<p align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/csharp/csharp-original.svg" width="40" height="40" alt="C#" title="C#"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/dotnetcore/dotnetcore-original.svg" width="40" height="40" alt=".NET" title=".NET Framework"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg" width="40" height="40" alt="MySQL Workbench" title="MySQL Workbench"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/apache/apache-original.svg" width="40" height="40" alt="XAMPP" title="XAMPP"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/visualstudio/visualstudio-original.svg" width="40" height="40" alt="Visual Studio" title="Visual Studio"/>
</p>



## Requisitos para funcionamento
### Instalação do Software XAMPP e MySQL Workbench
* Em **XAMPP Control Panel** Iniciar o módulo **"MySQL"**;
* Em **MySQL Connections** acessar o servidor local ou criar novo e configurar:

   **Connection Name:** _nomeDesejado_

   **Hostname:** 127.0.0.1

   **Port:** _porta indicada pelo XAMPP_

   **Username:** root

* Criar Banco de Dados nomeado 'sigosdb';
* Executar script de criação e população do Banco de Dados;

### Conectando o sistema com Banco de Dados
* Com o o projeto "SIGOS" aberto no *Visual Studio*, clique com o botão direito em "*Referências*" e selecione “**Manage NuGet Packages (Gerenciar Pacotes do NuGet).**”
* Na aba *Browse*, pesquise por **MySql.Data** , selecione o pacote oficial da Oracle e clique em Install;
* Na classe “Conexao.cs”, na linha do construtor (public Conexao()):

  ``` String dataSource = "datasource=localhost; username = root; password = '';" + "database='sigosdb';AllowZeroDateTime=true;";> ```

  **password:** Deixe em branco ("") se o **XAMPP** estiver com a senha padrão.

  **database:** Caso necessário, altere de 'sigosdb' para o nome do banco de dados criado.

**OBS:** Para a conexão ser válida e realizada, é necessário que os módulos “MySQL” esteja iniciado no **XAMPP**, com o status em verde. 


