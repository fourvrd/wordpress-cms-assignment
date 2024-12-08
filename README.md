## Uruchomienie kontenerów z Wordpressem oraz bazą danych

```bash
  docker compose up -d
```

Podczas uruchomienia, przy inicjalizacji kontener z bazą danych wczyta ostatniego dumpa znajdującego się w folderze `mysql-init`.
Strona będzie dostępna pod adresem `localhost:8080`.

## Dumpowanie bazy

```bash
  ./docker-mysqldump.sh
```

Podczas wykonywania tego skryptu, obecna zawartość bazy danych w kontenerze zostanie zdumpowana do pliku `wordpress_database.sql` w folderze `mysql-init`.
