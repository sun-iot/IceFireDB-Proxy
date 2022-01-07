![banner](./docs/logo.png)
# IceFireDB-Proxy
[![Build](https://github.com/IceFireDB/IceFireDB-Proxy/actions/workflows/main.yml/badge.svg)](https://github.com/IceFireDB/IceFireDB-Proxy/actions/workflows/main.yml) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![GitHub go.mod Go version](https://img.shields.io/github/go-mod/go-version/IceFireDB/IceFireDB-Proxy)](https://github.com/IceFireDB/IceFireDB-Proxy/blob/master/go.mod)    

IceFireDB-Proxy is a high performance Redis Proxy solution written in Go, including single node and cluster Proxy modes. Icefiredb-proxy detects request commands in real time and records logs and metrics for unstable keys, such as Big keys, hot keys, and slow keys, helping discover unreasonable data design and improving service stability.

## Table of Contents
- [Install](#Install)
- [Usage](#usage)
- [Command support](#command-support)
- [License](#license)

### Install
This project uses Go. Go check them out if you don't have them locally installed.
```text
1. Install Go
2. git clone https://github.com/IceFireDB/IceFireDB-Proxy.git $GOPATH/src/github.com/IceFireDB/IceFireDB-Proxy
3. cd $GOPATH/src/github.com/IceFireDB/IceFireDB-Proxy
4. make
```

### Usage
Run a binary file directly, if you need to run in the background can be added to the systemd system management
```shell
./bin/Icefiredb-proxy -c ./config/config.yaml
```

### Command support
#### String operating
* APPEND
* BITCOUNT
* BITPOS
* DECR
* DECRBY
* DEL
* EXISTS
* GET
* GETBIT
* SETBIT
* GETRANGE
* GETSET
* INCR
* INCRBY
* MGET
* MSET
* SET
* SETEX
* SETEXAT
* SETRANGE
* EXPIRE
* EXPIREAT
* TTL


#### Set operating
* SADD
* SCARD
* SETBIT
* SISMEMBER
* SMEMBERS
* SPOP
* SRANDMEMBER
* SREM
* SSCAN

#### List operating
* LINDEX
* LINSERT
* LLEN
* LPOP
* LPUSH
* LPUSHX
* LRANGE
* LREM
* LSET
* LTRIM
* RPOP
* RPUSH
* RPUSHX

#### hash operating
* HDEL
* HEXISTS
* HGET
* HGETALL
* HINCRBY
* HINCRBYFLOAT
* HKEYS
* HLEN
* HMGET
* HMSET
* HSCAN
* HSET
* HSETNX
* HSTRLEN
* HVALS

#### Sorted Sets 
* ZADD
* ZCARD
* ZCOUNT
* ZINCRBY
* ZLEXCOUNT
* ZPOPMAX
* ZPOPMIN
* ZLEXCOUNT
* ZRANGE
* ZRANGEBYLEX
* ZRANGEBYSCORE
* ZRANK
* ZREM
* ZREMRANGEBYLEX
* ZREMRANGEBYRANK
* ZREMRANGEBYSCORE
* ZREVRANGE
* ZREVRANGEBYLEX
* ZREVRANGEBYSCORE
* ZREVRANK
* ZSCAN
* ZSCORE

#### Stream operating
* XACK
* XADD
* XCLAIM
* XDEL
* XLEN
* XINFO
* XPENDING
* XRANGE
* XREADGROUP
* XREVRANGE
* XTRIM
* XGROUP


#### other operating

* COMMAND
* PING
* QUIT

### License
Icefiredb-proxy is under the Apache 2.0 license. See the [LICENSE](./LICENSE) directory for details.
