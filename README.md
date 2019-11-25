# NSQ Exporter

[![GoDoc](https://godoc.org/github.com/ueski/nsq_exporter?status.svg)](https://godoc.org/github.com/ueski/nsq_exporter) [![Build Status](https://travis-ci.org/ueski/nsq_exporter.svg?branch=master)](https://travis-ci.org/ueski/nsq_exporter) [![](https://images.microbadger.com/badges/image/ueski/nsq_exporter.svg)](https://microbadger.com/images/ueski/nsq_exporter "Get your own image badge on microbadger.com")

NSQ exporter for prometheus.io, written in go.

## Usage

    docker run -d --name nsq_exporter -l nsqd:nsqd -p 9117:9117 ueski/nsq_exporter:latest -nsqd.addr=http://nsqd:4151 -collect=stats.topics,stats.channels,stats.clients

## Building

    make

    OR

    go get -u github.com/ueski/nsq_exporter
    go install github.com/ueski/nsq_exporter

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request
