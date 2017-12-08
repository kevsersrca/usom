# Usom Url Scanner
Scan usom blocked url list inside your ip masks.

## Usage

```
go get -u github.com/kevsersrca/usom
```

## Example

```go


package main

import (
	"fmt"
	"time"
	s "github.com/kevsersrca/usom"
)

func main() {
	masks := []string{"89.43.28.0/22"}
	speed := 100
	list := s.Scan(masks, speed)
	for _, v := range list {
		fmt.Println(v.Hostname, v.IP)
	}
}


```
