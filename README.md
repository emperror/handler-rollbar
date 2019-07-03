# Rollbar handler

[![CircleCI](https://circleci.com/gh/emperror/handler-rollbar.svg?style=svg)](https://circleci.com/gh/emperror/handler-rollbar)
[![Go Report Card](https://goreportcard.com/badge/handler.emperror.dev/rollbar?style=flat-square)](https://goreportcard.com/report/handler.emperror.dev/rollbar)
[![GolangCI](https://golangci.com/badges/github.com/emperror/handler-rollbar.svg)](https://golangci.com/r/github.com/emperror/handler-rollbar)
[![GoDoc](http://img.shields.io/badge/godoc-reference-5272B4.svg?style=flat-square)](https://godoc.org/handler.emperror.dev/rollbar)

**Error handler integration for [Rollbar](https://rollbar.com).**


## Installation

```bash
go get handler.emperror.dev/rollbar
```


## Usage

```go
package main

import (
	"handler.emperror.dev/rollbar"
)

func main() {
    	token := "token"

	handler := rollbar.New(token, "env", "version", "host", "serverRoot")
}
```


## Development

When all coding and testing is done, please run the test suite:

``` bash
$ make check
```


## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.
