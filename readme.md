# Restful Api Laravel Passport

## Table of Contents

- [Installation](#installation)
- [Routes](#routes)
    - [Authentication](#authentication)


### Installation

1. Clone repository
```
$ git clone https://github.com/AhmedAltallaa/RestfulApi.git
```

2. Enter folder
```
$ cd RestfulApi
```

3. Install composer dependencies
```
~/RestfulApi$ composer install
```

4. Generate APP_KEY
```
~/RestfulApi$ php artisan key:generate
```

5. Configure .env file, edit file with next command `$ nano .env`
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=database
DB_USERNAME=user
DB_PASSWORD=secret
```

6. Run migrations
```
~/RestfulApi$ php artisan migrate
```

7. Create client
```
~/RestfulApi$ php artisan passport:install
```

### Routes

##### Authentication

- POST /auth/login
- GET /auth/logout
- POST /auth/signup
- GET /auth/signup/activate/{token}
- GET /auth/user
