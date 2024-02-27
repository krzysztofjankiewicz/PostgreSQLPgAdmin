# PostgreSQLPgAdmin

1. Skopuj repozytorium z zawartym w nim plikiem `docker-compose.yml`

```
git clone https://github.com/krzysztofjankiewicz/PostgreSQLPgAdmin.git
```

2. Dokonaj edycji pliku `docker-compose.yml`
    - koniecznie dostosuj lokalne katalogi, do których zostaną podmontowane katalogi z danymi PostgreSQL oraz PgAdmin
    - opcjonalnie zmień nazwy użytkowników 
    - opcjonalnie zmień hasła 
    - opcjonalnie zmień porty, pod którymi obie usługi (PostgreSQL oraz PgAdmin) będą dostępne  

3. Przejdź w terminalu do katalogu z plikiem `docker-compose.yml`

```
cd PostgreSQLPgAdmin
```

4. Uruchom oba kontenery 

```
docker-compose up -d
```
