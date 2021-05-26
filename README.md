## <center>APIDOK - DOK DESPACHANTE</center>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

API em Laravel que ir� devolver mensagens em formato JSON para um CRUD de usu�rio.
<br>Possui autentica��o JWT e cont�m tamb�m m�todos para login, logout e refresh do token.

<hr>

### Instru��es:

- Clonar o projeto
- Atualizar as depend�ncias:<br><br>
  <code>composer install</code>
  <br><br>
- Renomear arquivo <strong>.env.example</strong> para <strong>.env</strong>
- Gerar chave da aplica��o:<br><br>
  <code>php artisan key:generate</code>
  <br><br>
- Gerar secret do autenticador JWT:<br><br>
  <code>php artisan jwt:secret</code>
  <br><br>
- Criar base em MySql com nome <strong>apidoc</strong>. Recomendado utilizar collation UTF8MB4_UNICODE_CI
- Alterar as credenciais do seu banco no arquivo <strong>.env</strong>
- Executar a migration:<br><br>
  <code>php artisan migrate</code>
  <br><br>
- Subir o servi�o:<br><br>
  <code>php artisan serve</code>  

<hr>

### Funcionamento e Endpoits:

Recomendamos utilizar para os testes o site https://resttesttest.com/

- Verificar em <strong>routes/api.php</strong> os endpoints e par�metros exigidos.
- Somente a cria��o de usu�rio e login geram Token. Utilizar essas a��es para obter o token
e assim utiliz�-lo nas rotinas que exigem.
- O token expira em 60 minutos.


  

