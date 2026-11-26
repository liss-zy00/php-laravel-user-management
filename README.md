# Gestão de usuários em Laravel

CRUD de usuários em Laravel 8: listar, criar, ver, editar e apagar. Projeto de estudo.

## Rodar

Precisa de PHP 7.3+ (ou 8), Composer e um banco de dados (MySQL ou SQLite).

```bash
composer install
cp .env.example .env
php artisan key:generate
# ajuste DB_* no .env
php artisan migrate
php artisan serve
```

Abra http://localhost:8000/users.

## Rotas

| Método | Rota | O que faz |
|---|---|---|
| GET | `/users` | Lista os usuários |
| GET | `/users/create` | Formulário de cadastro |
| POST | `/users/create/store` | Salva um usuário |
| GET | `/users/show/{id}` | Mostra um usuário |
| PUT | `/users/show/update/{id}` | Atualiza |
| DELETE | `/users/show/delete/{id}` | Apaga |
