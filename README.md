# Rebloom Module plugin for node_redis

This package allows [node_redis](https://github.com/NodeRedis/node_redis) (2.8+) to interface with the Redis module [rebloom](https://github.com/RedisLabsModules/rebloom).

To use this module, you will need Redis 4.0 or higher and the rebloom module installed.

## Usage

```
var
   redis       = require('redis'),
   rebloom     = require('redis-rebloom');

rebloom(redis);
```

The ReBloom commands will be mapped to javascript-friendly names (`BF.ADD` becomes `client.bf_add`).