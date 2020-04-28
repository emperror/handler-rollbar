# Rollbar handler

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/emperror/handler-rollbar/CI?style=flat-square)](https://github.com/emperror/handler-rollbar/actions?query=workflow%3ACI)
[![Codecov](https://img.shields.io/codecov/c/github/emperror/handler-rollbar?style=flat-square)](https://codecov.io/gh/emperror/handler-rollbar)
[![Go Report Card](https://goreportcard.com/badge/emperror.dev/handler/rollbar?style=flat-square)](https://goreportcard.com/report/emperror.dev/handler/rollbar)
![Go Version](https://img.shields.io/badge/go%20version-%3E=1.12-61CFDD.svg?style=flat-square)
[![go.dev reference](https://img.shields.io/badge/go.dev-reference-007d9c?logo=go&logoColor=white&style=flat-square)](https://pkg.go.dev/mod/emperror.dev/handler/rollbar)


**Error handler integration for [Rollbar](https://rollbar.com).**


## Installation

```bash
go get emperror.dev/handler/rollbar
```


## Usage

```go
package main

import (
	"emperror.dev/handler/rollbar"
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
