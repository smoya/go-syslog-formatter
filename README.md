[![Go Report Card](https://goreportcard.com/badge/github.com/smoya/syslog-format)](https://goreportcard.com/report/github.com/smoya/syslog-format) 
![Build](https://github.com/smoya/syslog-format/workflows/Build/badge.svg)
[![License](https://img.shields.io/static/v1?label=license&message=MIT&color=blueviolet)](./LICENSE) 

# Repository archived. No longer actively maintained.

This project is not maintained anymore. I recommend you using https://github.com/influxdata/go-syslog/blob/develop/rfc5424/builder.go instead, which has all the features this library provided plus tons of others. It is also maintained by the InfluxDB engineering team, which ensures continuity on development.

# syslog-format
A syslog formatter Golang library.

## Standards
This library formats syslog messages according the [RFC5424](https://tools.ietf.org/html/rfc5424) and [RFC3164](https://tools.ietf.org/html/rfc3164).

## Installation
```
$ go get github.com/smoya/syslog-format
```

## Test
Coverage: https://gocover.io/github.com/smoya/syslog-format

## TODO
* Port [syslog](https://golang.org/pkg/log/syslog/) pkg dial functionality and adapt it with this formatter. The [syslog](https://golang.org/pkg/log/syslog/) only supports the RFC3164.
* Add support for multiple structured data chunks. Right now only supports one, with the name `context@{pid}`.
* Add support for standard structured data SD-ID. More info [here](https://tools.ietf.org/html/rfc5424#section-9.2).

