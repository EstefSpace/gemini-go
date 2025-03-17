# Gemini-Go

Un paquete de Golang muy sencillo, el cual facilita el uso de la API de Gemini. **Se requiere un API KEY de Google**.

# Instalación

```
go get github.com/estefspace/gemini-go
```

# Uso

```go
package main

import (
	"fmt"
	"github.com/estefspace/gemini-go"
)

func main() {
	prompt := "Cuentame la historia de Chicharito"
	client := gemini.NewClient("API_KEY")

	content, err := client.Ask(prompt)
	if err != nil {
		fmt.Println("Ocurrio un error")
	}

	fmt.Println(content)
}
```
