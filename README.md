<b>Projeto Spring Boot - Sistema de Pedidos</b> </br>
Java - Spring Boot

<b>Descrição</b> </br>
Este é um projeto <b>Spring Boot</b> que implementa um sistema básico de pedidos (e-commerce). </br>
O sistema inclui funcionalidades para gerenciar <b>usuários</b>, <b>produtos</b>, <b>categorias</b>, <b>pedidos</b> e <b>itens de pedidos</b>. </br> </br>

<b>O projeto foi desenvolvido para fins educacionais e demonstra o uso de conceitos como:</b>

<b>Spring Data JPA</b>: Para interação com o banco de dados. </br>
<b>Relacionamentos entre entidades</b>: Mapeamento de relacionamentos One-to-Many , Many-to-One e Many-to-Many . </br>
<b>Seed de dados</b>: Configuração de dados iniciais para facilitar testes. </br>
<b>Enumerações</b>: Uso de enums para representar estados de pedidos. </br>
<b>Injeção de dependência</b>: Utilização de @Autowired para integrar repositórios e serviços. </br> </br>

<b>Funcionalidades Principais</b> </br>
<b>Usuários</b>: Cadastro e gerenciamento de usuários. </br>
<b>Produtos</b>: Cadastro de produtos com categorias associadas. </br>
<b>Pedidos</b>: Criação de pedidos com status (Pago , Aguardando Pagamento ). </br>
<b>Itens de Pedido</b>: Associação de produtos a pedidos com quantidade e preço unitário. </br>
<b>Pagamentos</b>: Registro de pagamentos vinculados a pedidos. </br> </br>

<b>Pré-requisitos</b> </br>
Para executar este projeto, você precisará dos seguintes itens instalados em sua máquina:

<b>Java 17</b> ou superior </br>
<b>Maven</b> (para gerenciamento de dependências) </br>
<b>MySQL</b> (ou outro banco de dados suportado pelo Spring Data JPA) </br>
<b>Git</b> (opcional, para clonar o repositório) </br> </br>

<b>Configuração Inicial</b>
1. Clone o Repositório: git clone https://github.com/gui55gui/workshop-springboot3-jpa.git
2. Configuração do Banco de Dados:
Certifique-se de ter um banco de dados MySQL configurado. Edite o arquivo application.properties (localizado em src/main/resources) para ajustar as configurações de conexão:
spring.datasource.url=jdbc:mysql://localhost:3306/nome_do_banco?useSSL=false&serverTimezone=UTC
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
3. Executar o Projeto.

<b>Seed de Dados</b> </br>
O projeto inclui uma classe de configuração (<code>TesteConfig</code>) que insere dados iniciais no banco de dados ao iniciar a aplicação no perfil <code>test</code>. Os dados incluem: </br>

<b>Usuários</b>: Maria Brown e Alex Green. </br>
<b>Categorias</b>: Eletrônicos, Livros e Computadores. </br>
<b>Produtos</b>: Exemplos como "The Lord of the Rings", "Smart TV" e "Macbook Pro". </br>
<b>Pedidos</b>: Três pedidos com diferentes status (Pago , Aguardando Pagamento ). </br>
<b>Itens de Pedido</b>: Produtos associados aos pedidos com quantidades e preços. </br>
