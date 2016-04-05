# Golang编译时自动指定版本信息

## 使用

``` go
package main

import (
	"fmt"
)

var (
	Version = "None"
)

func main() {
	fmt.Printf("App Version:%s", Version)
}
```

## 编译

``` bash
$ go build -ldflags "-X main.Version=0.1.0" -o demo
```

## 输出

``` bash
$ ./demo
```
```
App Version:0.1.0
```