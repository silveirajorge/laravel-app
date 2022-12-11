
# Setup Docker Para Projetos Laravel

### Passo a passo
Clone Repositório
```sh
git clone https://github.com/laravel/laravel.git my-project
```
```sh
cd my-project/
```


Remova o versionamento (opcional)
```sh
rm -rf .git/
```


Crie o Arquivo .env
```sh
cp .env.example .env
```


Atualize as variáveis de ambiente do arquivo .env
```dosini
DB_CONNECTION=mysql
DB_HOST=laravel-db
DB_PORT=3306
DB_DATABASE=nome_que_desejar
DB_USERNAME=nome_que_desejar
DB_PASSWORD=nome_que_desejar
DB_ROOT_PASSWORD=nome_que_desejar
```


Suba os containers do projeto
```sh
docker-compose up -d
```


Acesse o container app com o bash
```sh
docker-compose exec app bash
```


Instale as dependências do projeto
```sh
composer install
```


Gere a key do projeto Laravel
```sh
php artisan key:generate
```


Acesse o projeto
[http://localhost](http://localhost)