# plist - A pure Go property list transcoder [![coverage report](https://gitlab.howett.net/go/plist/badges/master/coverage.svg)](https://gitlab.howett.net/go/plist/commits/master)
## INSTALL
```
$ go get github.com/ironsalsa/go-plist
```

## FEATURES
* Supports encoding/decoding property lists (Apple XML, Apple Binary, OpenStep and GNUStep) from/to arbitrary Go types

## USE
```go
package main
import (
	"github.com/ironsalsa/go-plist"
	"os"
)
func main() {
	encoder := plist.NewEncoder(os.Stdout)
	encoder.Encode(map[string]string{"hello": "world"})
}
```
