<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	testcollab5 "github.com/speakeasy-sdks/test-collab-5"
	"log"
	"net/http"
)

func main() {
	s := testcollab5.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->