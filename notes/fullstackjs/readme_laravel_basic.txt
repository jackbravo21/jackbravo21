composer global require "laravel/installer"				//instalador global;
laravel new nome_do_projeto							    //caso vc use o install acima;
composer create-project --prefer-dist laravel/laravel nome_do_projeto "5.5.*"	//instalador do laravel;

php artisan key:generate							    //laravel gera essa chave quando instala;
php artisan serve								        //para rodar o laravel, ele informa a porta no console;
.env										            //arquivo de config do server, etc;
/nome_projeto/config/app.php							//contem os dados do projeto, como nome do projeto, url do domínio, key da .env;
//verificar no app.php se tem a chave "key" com o base65 que pega no .env/APP_KEY;
/nome_projeto/config/database.php						//configura o tipo de db que vai usar;

Dentro de:
/projeto/app/Http                                       //tem os controllers, middlewares, providers;
/middleware/verifyCsrfToken.php                         //verifica o token, eh o token de formulario;
/http/kernel.php                                        //tem a configuracoes das pastas, exemplo: Middleware, arquivo de config que colocamos na principal de cada tipo;
/projeto/routes/                                        //ficam as rotas, as rotas sao dividas para web(sistema url na web), via api(webserver), e console;
/app/provirders/                                        //ficam as autenticacoes, services, etc;
/app/Http/Middleware/                                   //fica o auth das rotas;
/app/Http/Kernel.php                                    //onde ficam registrados os middlewares;
/bootstrap/                                             //arquivo de inicializacao da aplicacao;
/config/                                                //onde ficam todas as config, emails, arquivos, cache, etc;
/database/factories/                                    //ficam as factories do projeto, podendo gerar usarios com o faker;
/database/migrations/                                   //onde ficam as tabelas dos bancos;
/database/seeds/                                        //semeadora que cria varios registros;
/public/                                                //pasta root, eh onde coloca o css, js, etc... eh o doccumentRoot;
/resources/                                             //contem as views, assets que contem js e sass;
/vendor/                                                //eh o que contem todo framework, como .env, .gitignore, etc;

