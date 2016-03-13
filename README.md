# ssg
- Self Signed *certificate* Generator

This code is adapted straight out of the Go standard library code
Original source: crypto/tls/generate_cert.go

I find it nice to use while spining up HTTP2 servers locally real quick and
need a certificate plus private key instead of running through a ritual with openssl on the commandline.

## Usage
```shell
$ go get github.com/odeke-em/ssg
$ ssg --host example.com
```

That will write files `cert.pem` and `keys.pem`  in your current working directory, overwriting any existing files with the same names.

## LICENSE
Copyright 2009 The Go Authors. All rights reserved.
