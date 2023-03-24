# Installing dependencies
```bash
go mod tidy
```
# For running service

```bash
go run main.go
```

# you can make request to 

## GET ALL, POST

[http://localhost:3001/api/notes](http://localhost:3001/api/notes)

## PUT, GET BY ID
[http://localhost:3001/api/notes/{id}](http://localhost:3001/api/notes/{id})

## Home page
[http://localhost:3001/](http://localhost:3001/)


# For testing 
Now generate report
```bash
go test -coverprofile=coverage2.txt -covermode count ./
```
Now generate xml
```bash
/home/$USER/go/bin/gocover-cobertura < coverage.txt > coverage.xml
```