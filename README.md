# ProgrammingGoodies

## Github

### Adding existing project to Github
```git init```

```git add .``` or ```git add -A```

```git commit -m "Initial Commit"```

```git push origin master```

### Track specific file
```git add [file]```

### Untrack specific file
```git rm -r --cached [file]```

### Untrack all files
```git rm -r --cached *```

## ASPNETCORE
### Production publish
```dotnet publish --configuration Release```

### Production run localhost url
```dotnet [name].dll --urls="http://localhost:5000"```

**_Do NOT use ```dotnet run``` in production_**

## Linux
### Setup service
In ```/etc/systemd/system``` create a file ```myapp.service```:
```
[Unit]
Description=My application description

[Service]
WorkingDirectory=/usr/share/myapp
ExecStart=/usr/bin/dotnet /usr/share/myapp/myapp.dll
SyslogIdentifier=myapp
User=www-data

[Install]
WantedBy=multi-user.target
```

### Add/Start service
```
systemctl enable myapp
systemctl start myapp
```

### Stop/Remove service
```
systemd stop myapp
systemd disable myapp
```

## Curl

### All (headers & response output)
```curl -v [url]```

### Response output
```curl -o - [url]```
