# pgsql-sheet
## Enable remote access
### Centos

#### Change listening addresses
```vi /var/lib/pgsql/data/postgresql.conf```

```listen_addresses='*'```


#### Restart
```sudo systemctl restart postgresql```
