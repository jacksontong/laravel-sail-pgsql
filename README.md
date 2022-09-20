Create `.env` file

```bash
./vendor/bin/sail up -d
./vendor/bin/sail artisan key:generate
```

Update database config in `.env` file

```
DB_CONNECTION=pgsql
DB_HOST=pgsql
DB_PORT=5432
DB_DATABASE=laravel_pgsql
DB_USERNAME=sail
DB_PASSWORD=password
```

Run

```
./vendor/bin/sail artisan migrate
```
