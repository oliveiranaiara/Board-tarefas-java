📋 Board de Tarefas em Java
Este projeto é uma aplicação de terminal para gerenciamento de tarefas, desenvolvida em Java com JDBC e MySQL. A estrutura segue o padrão em camadas (Model, Repository, Service, UI) e permite a criação de boards, colunas e cards, além do rastreamento de tempo e geração de relatórios.

🛠️ Tecnologias
Java 17+

JDBC

MySQL

Maven

IntelliJ IDEA (recomendado)

Terminal (interface via linha de comando)

📁 Estrutura do Projeto
model/ – Entidades como Board, Card, Column, TimeEntry

repository/ – Acesso a dados com JDBC

service/ – Regras de negócio

ui/ – Menus e interações via terminal

resources/ – Configurações do banco

🚀 Funcionalidades
Criar, listar, selecionar e excluir boards

Criar, listar e excluir colunas

Criar, mover, editar e excluir cards

Iniciar/parar time tracking por tarefa

Gerar relatório de tempo por board e card

⚙️ Configuração do Ambiente
1. Clone o repositório
bash
Copiar
Editar
git clone https://github.com/oliveiranaiara/Board-tarefas-java.git
cd Board-tarefas-java
2. Configure o banco de dados MySQL
Crie um banco de dados chamado board_db e execute o script de criação das tabelas em resources/db/init.sql (se disponível).

sql
Copiar
Editar
CREATE DATABASE board_db;
3. Atualize as credenciais do banco
Altere o arquivo resources/db.properties com seu usuário e senha do MySQL:

properties
Copiar
Editar
db.url=jdbc:mysql://localhost:3306/board_db
db.user=seu_usuario
db.password=sua_senha
4. Compile e execute o projeto
Use o Maven para compilar e executar:

bash
Copiar
Editar
mvn compile
mvn exec:java -Dexec.mainClass="ui.Menu"
🧪 Exemplo de Uso
Escolha um board ou crie um novo

Adicione colunas como "To Do", "Doing", "Done"

Crie cards com descrições

Use a opção de iniciar/parar tempo para acompanhar o progresso

📌 Requisitos
Java 17+

MySQL 8+

Maven 3.8+

📄 Licença
Este projeto está sob a licença MIT - veja o arquivo LICENSE para detalhes.

