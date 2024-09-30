<h1 align="center">  
  Documentação das Decisões Técnicas  
  <br/>  
</h1>  
 

<hr>

<h2>Resumo</h2>  

<p>  
O projeto foi organizado em uma estrutura de camadas para manter a separação de responsabilidades e facilitar a manutenção do código.  
</p>

<h2>Estrutura do Projeto</h2>  
<ul>  
  <li><strong>Apresentação</strong>: Responsável por orquestrar a aplicação e iniciar os serviços necessários.</li>  
  <li><strong>RPA</strong>: Contém a lógica de automação de tarefas usando Selenium WebDriver.</li>  
  <li><strong>Domínio</strong>: Define as entidades de negócio.</li>  
  <li><strong>Infraestrutura</strong>: Camada de persistência de dados usando Dapper e acesso ao banco de dados MySQL.</li>  
  <li><strong>Injeção de Dependência</strong>: Configuração central para DI.</li>  
</ul>  

<hr>

<h2>Decisões Técnicas</h2>  
<h3>2.1. Escolha do Selenium WebDriver</h3>  
<p>  
O Selenium WebDriver foi escolhido para automação de tarefas na web, pois oferece suporte a várias linguagens de programação e navegadores, e lida bem com páginas dinâmicas.  
</p>

<h3>2.2. Uso do Dapper para Persistência de Dados</h3>  
<p>  
Dapper foi escolhido por ser leve e permitir controle direto sobre as consultas SQL, sendo mais adequado ao projeto.  
</p>

<h3>2.3. Banco de Dados MySQL</h3>  
<p>  
MySQL foi escolhido por sua robustez e facilidade de integração com Dapper.  
</p>

<h3>2.4. Injeção de Dependências</h3>  
<p>  
A DI permite que as dependências sejam facilmente substituídas e injetadas no código, facilitando a manutenção.  
</p>

<h3>2.5. Git Flow</h3>  
<p>  
O Git Flow foi adotado para organização das branches, com desenvolvimento paralelo e controlado.  
</p>

<hr>

<h2>Fluxo da Aplicação</h2>  

<ul>  
  <li><strong>Execução de Busca com Selenium</strong>: O Selenium realiza a automação e coleta dados.</li>  
  <li><strong>Persistência com Dapper</strong>: Os dados coletados são persistidos no banco MySQL.</li>  
  <li><strong>Tratamento de Erros</strong>: Erros são tratados para manter o fluxo de forma controlada.</li>  
</ul>  

<hr>

<h2>Tratamento de Erros e Casos Inesperados</h2>  
<p>  
O sistema lida com falhas no Selenium e problemas de conexão com o MySQL de forma robusta, para garantir que o fluxo não seja interrompido.  
</p>

<hr>

<h2>Decisão de Não Usar Entity Framework</h2>  
<p>  
Dapper foi escolhido em vez de Entity Framework por ser mais leve e adequado ao controle direto de SQL.  
</p>

<hr>

<h2>Instruções de Instalação</h2>  

<p>Siga os passos abaixo para clonar e executar o projeto:</p>

<h3>🛠 Instalação</h3>  

<ol>  
  <li>Clone o repositório:  
   <code>git clone https://github.com/lesistemas/AluraSearch.git</code>  
  </li>  
  <li>Instale as dependências necessárias, incluindo:  
    <ul>  
      <li>Selenium WebDriver</li>  
      <li>Dapper</li>  
      <li>MySQL</li>  
    </ul>  
  </li> 
