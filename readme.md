# PostgreSQLPgAdmin

1. Skopuj repozytorium z zawartym w nim plikiem `docker-compose.yml`

```sh
git clone https://github.com/krzysztofjankiewicz/PostgreSQLPgAdmin.git
```

2. Dokonaj edycji pliku `docker-compose.yml`
    - **koniecznie** dostosuj lokalne katalogi, do których zostaną podmontowane katalogi z danymi PostgreSQL oraz PgAdmin
    - opcjonalnie zmień nazwy użytkowników 
    - opcjonalnie zmień hasła 
    - opcjonalnie zmień porty, pod którymi obie usługi (PostgreSQL oraz PgAdmin) będą dostępne  

3. Przejdź w terminalu do katalogu z plikiem `docker-compose.yml`

```sh
cd PostgreSQLPgAdmin
```

4. Uruchom oba kontenery 

```sh
docker-compose up -d
```

5. Pod adresem `http://localhost:15432/` (dla domyślnego portu) dostępny jest PgAdmin. 
    - użytkownik: `admin@pgadmin.com` (domyślnie)
    - hasło: `postgres` (domyślnie)

6. Baza danych PostgreSQL dostępna jest zgodnie z poniższymi własnościami
    - host: `postgres` (domyślnie)
    - użytkownik: `postgres` (domyślnie)
    - hasło: `postgres` (domyślnie)

## Dodatkowe uwagi

PgAdmin udostępnia domyślnie pliki (np. skrypty) z katalogu `/var/lib/pgadmin/storage/<username>`.
W naszym przypadku jest to katalog hosta: `C:\DockerVolumes\PgAdmin\storage\admin_pgadmin.com` (domyślnie) 