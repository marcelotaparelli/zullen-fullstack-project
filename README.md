# zullen-fullstack-project
<h3>Projeto Fullstack (CRUD) para um contraturno escolar feito em .NET, Angular e, posteriormente, em Blazor. (repositório privado)</h3>

Primeiramente, busquei ver as necessidades da usuária do sistema e quais informações seriam mais relevantes para armazenar. Com isso, pude definir meu Modelo/Classe/Entidade e suas propriedades.

<img src="models.jpg">

Segui o modelo de uma Classe "Resposta de Serviço" no qual este dados seriam inseridos numa propriedade "Dados", acompanhados de uma descrição booleana "Sucesso" para indicar o status das operações e os detalhes em uma string "Mensagem". 

<img src="response.jpg">

Com os Modelos definidos, criei o Contexto do Banco de Dados usando o Entity Framework, configurei a conexão com o Banco de Dados (SQL Server) no appsettings.json adicionando os devidos serviços em Program.cs e realizei as migrações.

<img src="dbContext.jpg">

A próxima etapa foi a criação dos Endpoints através de um Serviço e do Controlador e suas respectivas lógicas.

<img src="controller.jpg">

<img src="api.jpg">

Para o Frontend inicial utilizei Angular.

<img src="angular.jpg">

Esta foi a primeira etapa do denvolvimento.

<br><br><br>

<h3>Transferência do Frontend para Blazor, criação de um novo Model e Banco de Dados para os afazeres e criação do sistema de autenticação/autorização</h3>

Utilizei fontes e cores condizentes com o logo da empresa buscando harmonizar o design da interface. Nesta etapa, o produto está como segue rodando em Docker Containers.

<img src="blazor-login.jpg">

<img src="home.jpg">

<img src="adicionar.jpg">

<img src="detalhes.jpg">

<img src="editar.jpg">

<img src="todo.gif">

<h3>A etapa presente consiste em implementar uma área de agendamento de vagas para o contraturno</h3>

Alterei a propriedade "dias" do tipo "integer" (que antes armazenava o numero de dias por semana que a criança viria) para uma Lista de "strings" contendo os dias da semana que criança virá.

<img src="diasDaSemana.jpg">

Para o calendário estou testando o repositório do <a href="https://github.com/danheron/Heron.MudCalendar/">danheron</a> e já adicionei a lógica para as crianças aparecerem no calendário de acordo com o turno cadastrado:

<img src="calendario.jpg">

<li>O próximo passo será fazer a lógica para as crianças aparecerem nos dias da semana cadastrados</li>





