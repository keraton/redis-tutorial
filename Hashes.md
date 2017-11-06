# Hashes

Hashes is like a key-value within a key-value.

## Commands
### hset
Sets field in the hash stored at key to value. 
If key does not exist, a new key holding a hash is created. 
If field already exists in the hash, it is overwritten.

```
redis> HSET myhash field1 "Hello"
(integer) 1
redis> HGET myhash field1
"Hello"
redis> 
```


## Reference
See others related hashes commands here : https://redis.io/commands/hset
