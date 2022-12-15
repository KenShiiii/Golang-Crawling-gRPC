# proto 
add this line for go code
```proto
option go_package = "<package path>";
```


## compile proto: message
``protoc --go_out=echo  echo/echo.proto``


## compile proto: grpc service
``protoc --go-grpc_out=echo  echo/echo.proto``

<br>

### if import can't be find in the generated pb.go file.
```
go mod tidy
```