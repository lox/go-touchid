# Authenticating with TouchID

```golang
package main

import (
  "log"

  touchid "github.com/lox/go-touchid"
)

func main() {
  ok, err := touchid.Authenticate("access llamas")
  if err != nil {
    log.Fatal(err)
  }

  if ok {
    log.Printf("Authenticated")
  } else {
    log.Fatal("Failed to authenticate")
  }
}
```
