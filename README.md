# Usom Url Scanner
Scan usom blocked url list inside your ip masks
use Usom method for all 
use UsomDaily method today 

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
	list := s.Usom([]string{"89.43.28.0/22"}, time.Millisecond*100)
	for _, v := range list {
		fmt.Println(v.Hostname, v.IP)
	}
}


```