## String

String is the most basic key - value in Redis database.
Store a "String" (or a binary) and reference it with a key.

## Basic commands

### SET
Set key to hold the string value. If key already holds a value, it is overwritten.

```
redis> SET mykey "Hello"
"OK"
redis> GET mykey
"Hello"
redis> 

```

Overwrite.

```
redis> SET mykey "Bonjour"
"OK"
redis> GET mykey
"Bonjour"
redis> 

```

## GET 

Get the value of key. If the key does not exist the special value nil is returned

## APPEND

If key already exists and is a string, this command appends the value at the end of the string.

```
redis> EXISTS mykey
(integer) 0
redis> APPEND mykey "Hello"
(integer) 5
redis> APPEND mykey " World"
(integer) 11
redis> GET mykey
"Hello World"
redis> 

```

## Reference
See others related to the set command here.
https://redis.io/commands/set
