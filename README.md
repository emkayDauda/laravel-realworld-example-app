## Getting started

You'll need [Docker](https://docs.docker.com/get-docker/) under Linux / macOS (or Windows WSL2) and docker-compose.

### Installation

Clone the repository and change directory:

    git clone https://github.com/emkayDauda/laravel-realworld-example-app.git
    cd laravel-realworld-example-app

Copy .env.example into .env

```
    cp .env.example .env
```

Build and start the project up using docker (you might need sudo privileges if you run this in an ec2 instance)
```
    docker-compose build app
    docker-compose up -d
```

Next, run the startup script provided in the repo (again, you might need sudo)
```
    chmod +x startup.sh
    ./startup.sh
```

Finally, go to your host ip address (or localhost if running on your computer) and you should see the laravel welcome page.

Check the endpoints to confirm the database works and has been seeded e.g `localhost/api/articles` or `<ip-address>/api/articles`

# ![Laravel RealWorld Example App](.github/readme/logo.png)
