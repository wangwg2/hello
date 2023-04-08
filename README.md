## hello.go
创建一个名为 `hellogo.go` 的文件

[hellogo.go](hellogo.go)

通过 `go` 工具运行它
```bash
go mod init github.com/wangwg2/hellogo
go run hellogo.go

# output
Hello, Welcome to Go
```

## go workspace

在 `hellogo` 同级目录 创建 `stringutil`

修改 `hellogo.go` 使用 `stringutil`


在 workspace 目录(`demows`) 运行
```bash
# 设置
go work init ./hellogo
go work use ./stringutil
# 运行 hellogo
go run github.com/wangwg2/hellogo
```
