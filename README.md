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
```dotnet publish```

### Production run localhost url
```dotnet [name].dll --urls="http://localhost:5000"```

## Curl

### All (headers & response output)
```curl -v [url]```

### Response output
```curl -o - [url]```
