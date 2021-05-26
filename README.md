# Spring-MVC
Criando uma loja online e interligando ao Banco de Dados através do Spring-MVC.

1. @Configuration e @EnableWebSecurity na classe que define as regras de segurança
As regras de acesso foram definidos pelo HttpSecurity
Os dados do usuário, como login e senha, foram definidos pelo método userDetailsService()
O login pode ser implementado de várias formas
Vimos a forma HttpBasic e form-login
A lógica de login e logout já está implementada pelo Spring Security, basta configurar

2.Executar uma autenticação baseada em JDBC
Criptografar a senha do usuário
Criar o modelo JDBC para representar o usuário e as permissões com Spring Security
Acessar o usuário autenticado com Spring MVC, usando o Principal
Escrever uma query JPA com Spring Data
Usar links relativos com Thymeleaf, por exemplo th:action="@{/pedido/novo}"
Desabilitar o CRSF (cross-site request forgery) com Spring Security

3.Separar a página pública (sem login) das páginas restritas
Redirecionar após logout para a página home
Trabalhar com paginação e ordenação, usando as classes Pageable e Sort
Usar o cache na aplicação para melhorar o desempenho usando a anotação @Cacheable

4.Criar um controlador específico para requisições REST
Usar o conceito REST para construir uma API devolvendo JSON
Usamos a anotação @RestController
Vimos que o Spring gera automaticamente o JSON

5.Construir uma página HTML com Vue.js
Executar requisições AJAX com Axiom
Vimos como consumir dados e enviar dados do form e JavaScript

6.Como recuperar valores de um formulário pelo JavaScript
Como enviar uma requisição AJAX do tipo POST com Axiom
Como fazer um tratamento de erro client-side e apresentar mensagens de erro
No lado do Spring MVC, vimos a anotação @ResquestBody, para receber o corpo da requisição e mapear os dados para um objeto do nosso domínio.

7.Que interceptadores ajudam a centralizar código que é comum para várias classes da mesma camada
Centralizando, facilitamos a manutenção desse código
Como criar um interceptador, estendendo a classe HandlerInterceptorAdaptor e registrando no InterceptorRegistry
A partir dessas classes, devemos sobrescrever os métodos em questão, como preHandle ou afterCompletion
Que um interceptador pode parar o fluxo da requisição
