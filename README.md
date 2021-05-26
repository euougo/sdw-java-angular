###### sdw-java-angular
# Santander Dev Week - Java + Angular

### Projeto: Tela de cotações - Santander

### Aula 1: Configurando Ambiente.

#### Back-end: 
1. Instalar JDK (Oracle JDK 8).
2. Instalar intelliJ.
3. Configurar intelliJ.

#### Front-end:
1. Node.js (LTS 14.16.1).
    ```
    node -v
    npm -v 
    ```
2. Visual Studio Code.
    - Desabilitar mini-map.
    - Mudar o terminal de cmd to git bash.
    - Extensões:
        - Angular Language Service.
        - TSLint.
    - Extensões opcionais:
        - EditorConfig for VS Code.
        - Atom One Dark Theme.
        - Material Icon Theme.
        - Auto Import.
        - Rainbow Brackets.
        - px to rem.

3. Angular CLI.
    ```
    npm install -g @angular/cli
    ng -version
    ng --version
    ng new hello-angular
    cd hello-angular
    ng serve --open
    ```
### Aula 2: Criação de uma API usando Spring Boot (Spring Web).

#### Criação projeto base (Back-end)

#### Objetivos
1. Criar o projeto base (Spring Boot / Maven)
    * https://start.spring.io/
    * spring initializr
        * Project: Maven Project
        * Language: Java
        * Spring Boot: 2.5.0
        * Project Metadata:
            * Group: com.project
            * Artifact: bootcamp
            * Name: bootcamp
            * Description: Backend criado para o bootcamp
            * Package name: com.project.bootcamp
            * Packaging: jar
            * Java: 8
        * Dependencies: Spring Web
2. Configurar o projeto base
    * renomeou arquivo application extension to .yml, esse arquivo fica na pasta resources
    * no application.yml setou o localhosto para a porta 8080 e no path bootcamp
3. Executar o projeto base
    * rodou a classe BootcampApplication em localhost na porta 8080 como configurado no arquivo application.yml
4. Criando as primeiras API's
    * Objetivos:
        a. Aprender REST / API / JSON
        b. Criar a camada controller
        c. Criar as api's
        d. Documentar api's
        ```
        <dependency>
			<groupId>org.springdoc</groupId>
			<artifactId>springdoc-openapi-ui</artifactId>
			<version>1.5.9</version>
		</dependency>
        ```
    * REST: O que é Rest (Representational State Transfer)?
        Definição de características fundamentais para a construção de aplicações Web seguindo boas práticas.
    * API: O que é API (Application Programming Interface)?
        Conjunto de rotinas e padrões estabelecidos e documentados por uma determinada aplicação.
    * Métodos:
        * GET - Obter um recurso
        * POST - Criar um recurso
        * PUT - Atualizar um recurso
        * DELETE - Remover um recurso
    * Code Responses:
        * 1XX - Informações Gerais
        * 2XX - Sucesso
        * 3XX - Redirecionamento
        * 4XX - Erros relacionados ao tratamento dos dados no servidor
        * 5XX - Erro no servidor
    * JSON
        JSON é basicamente um formato leve de troca de informações / dados entre sistemas.
        ```
        {
            "firstName": "Jonathan",
            "lastName": "Freeman",
            "loginCount": 4,
            "isWriter": true,
            "worksWith": ["Spantree Technology Group", "InfoWorld"],
            "pets": [
                {
                    "name": "Lilly",
                    "type": "Raccoon"
                }
            ]
        }
        ```
    * OpenAPI Swagger: http://localhost:8080/bootcamp/swagger-ui.html
5. Aplicando validações de dados:
    * Dependendencia:
        ```
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-validation</artifactId>
        </dependency>
        ```
    












































