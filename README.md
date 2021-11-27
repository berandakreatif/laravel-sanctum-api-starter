"# laravel-sanctum-api-starter"
Specification

-   Laravel 8
-   laravel/sanctum 2.12
-   MySQL Database

#How To Implement

-   Clone This Repo using terminal/command prompt "git clone https://github.com/berandakreatif/laravel-sanctum-api-starter.git"
-   Composer Install
-   Create MySQL Database
-   Edit/Create .env file with your db credential
-   php artisan migrate
-   php artisan serve (to running laravel)

#How To Use

-   REGISTER USER
    [POST] http://127.0.0.1:8000/api/register
    PARAMS :
    ##Header
    Accept application/json
    ##body
    name [your name]
    email [your email]
    password [your password]
-   LOGIN USER
    [POST] http://127.0.0.1:8000/api/token
    PARAMS :
    ##Header
    Accept application/json
    ##body
    email [your email]
    password [your password]

-   REFRESH TOKEN
    [POST] http://127.0.0.1:8000/api/token
    PARAMS :
    ##Header
    Accept application/json
    Authorization Bearer [your token here]
    ##body
    email [your email]
    password [your password]
