SISTEMA DE GERENCIAMENTO DE CLIENTES  

Aplicativo CRUD com Spring Boot (backend) e Angular (frontend).  

ESTRUTURA  
- frontend/ (submódulo Angular)  
- backend/ (submódulo Spring Boot)  

COMO CLONAR  
git clone --recurse-submodules https://github.com/ThiagoGoetten/crud.pontta.git 

REQUISITOS  
- JDK 8+, Node.js, Angular CLI, MySQL, Maven, Git  

CONFIGURAÇÃO DO BANCO  
1. CREATE DATABASE pontta_crud;  
2. Configure backend/src/main/resources/application.properties:  
   spring.datasource.url=jdbc:mysql://localhost:3306/pontta_crud  
   spring.datasource.username=seu_usuario  
   spring.datasource.password=sua_senha  
   spring.jpa.hibernate.ddl-auto=update  

EXECUTAR BACKEND  
1. cd backend  
2. mvn spring-boot:run  
3. Disponível em http://localhost:8080  

EXECUTAR FRONTEND  
1. cd frontend  
2. npm install  
3. ng serve  
4. Acesse http://localhost:4200  

TESTE  
- Criar, listar, atualizar e excluir clientes  
- Interface web em http://localhost:4200  

ATUALIZAR SUBMÓDULOS  
git submodule update --remote frontend  
git submodule update --remote backend  

SOLUÇÃO DE PROBLEMAS  
- Backend: Verifique banco de dados e portas  
- Frontend: Confirme backend rodando e URL da API  
- Submódulos: git submodule update --init --recursive  

REPOSITÓRIOS ORIGINAIS  
- Frontend: https://github.com/ThiagoGoetten/front.teste.pontta.git  
- Backend: https://github.com/ThiagoGoetten/back.teste.pontta.git  
