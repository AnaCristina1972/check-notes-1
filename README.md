# check-notes
Repositório destinado a disciplina de Engenharia de Aplicações Web

# Representação da Arquitetura
 
O princípio básico do MVC é a divisão da aplicação em três camadas: a camada de interação do usuário (view), a camada de manipulação dos dados (model) e a camada de controle (controller). Sendo possível
separar o código relativo à interface do usuário das regras de negócio. Os papéis de cada camada, são:
 
•               Model - a responsabilidade dos models é representar o negócio. Também é responsável pelo acesso e manipulação dos dados na sua aplicação. 
 
•               View - é responsável pela interface que será apresentada, mostrando as informações do model para o usuário.
 
Controller - é a camada de controle, responsável por ligar o model e a view, fazendo com que os models possam ser repassados para as views e vice-versa. A figura abaixo mostra o desenho arquitetural do MVC 


![MVC](https://github.com/AnaCristina1972/check-notes-1/blob/main/MVC.jpg)

## Visão Lógica
 
  ### Estrutura das Camadas
 
 
Camada Model
 
Essa camada conterá todas as interações necessárias para integrar o banco de dados com os objetos da view através do controller, onde separa todo tipo de SQL ou linguagens padrões de banco de dados, da camada view. 
 
 
Camada View
 
 
Essa camada conterá todas as interfaces visuais, na qual interagirá diretamente com o usuário do sistema. E estará subdividida em:  
 
Visual: contém a página Web, os formulários, e as referências adequadas para Designer.
 
Controles: Contém todos os códigos necessários para comunicação entre a camada de controller ou model, com a página Web (Ajax).
 
 
Camada Controller
 
Essa camada conterá os controladores necessários para interagir com a camada view com a camada model. Esses controladores servem como intermediários entre as duas outras camadas. A interação deve ser realizada quando houver uma aquisição da camada view.
 
 
## Visão de Implantação
 
Os sistemas são distribuídos da seguinte forma:
 
●  Servidores Web
●  Servidor de Intranet
 
Estrutura Lógica do funcionamento dos hardwares
 
Segurança
 
A aplicação deverá estar organizada de forma a conseguir separar fisicamente a interface da camada model. Buscando assim, dar uma maior segurança a aplicação.
 
Manutenibilidade
 
A aplicação deverá estar nas melhores práticas de implementação para que as manutenções sejam feitas de forma breve, e também se adequando e suportando novos ambientes.
 
8.1 Visão Geral
 
Fluxo de comunicação entre os modelos de classes criadas.
 
Conexão com o Banco de dados
É criada uma classe e uma função responsável por manter a interação entre o banco de dados e a camada view e controller. Sendo a classe e a função:
 
●  Conectar: Responsável por manter os dados do servidor, usuário, senha e o banco de dados que deseja fazer a conexão;
 
●  Conexão: Responsável por fazer a conexão com o banco de dados ;
 
 
## Visão de Implementação
 
View
 
Web<Sistema>(Index.php)
Web Services
 
Controller
 
ne<Sistema>(Biblioteca de Classes) se<Sistema>(Biblioteca de Classes) pe<Sistema>(Biblioteca de Classes)
ce<Sistema> (Biblioteca de Classe)
 
Model
 
Web Services
ws<Sistema> (Serviços web)
WCF
Bs<Sistema> (Biblioteca de Serviços)
Host
sw<Sistema> (Instalador serviço Windows)
13
hs<Sistema> (Host de aplicação IIS)
