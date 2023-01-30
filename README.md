# pgsql-sheet
## Enable remote access
### Centos

#### Change listening addresses
```
vi /var/lib/pgsql/data/postgresql.conf
```

```
listen_addresses='*'
```
#### Give access to all dbs in pg_hba.conf
```
host  all  all 0.0.0.0/0 md5 
```

#### Restart
```
sudo systemctl restart postgresql
```

## Postgres shell
```
sudo -i -u postgres
```

```
psql
```

## Change password
```
sudo -u postgres psql
```
```
\password postgres
```
## Restore DB
```
psql database_name < database_name_20160527.sql
```
