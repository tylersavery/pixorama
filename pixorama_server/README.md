# pixorama_server

This is the starting point for your Serverpod server.

To run your server, you first need to start Postgres and Redis. It's easiest to do with Docker.

    docker compose -p pixorama up --build --detach

Run migrations

    dart bin/main.dart --apply-migrations

Then you can start the Serverpod server.

    dart bin/main.dart

When you are finished, you can shut down Serverpod with `Ctrl-C`, then stop Postgres and Redis.

    docker compose stop
