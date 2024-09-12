# Documentation
[Official docs](https://redis.io/docs/latest/develop/data-types/strings/)

# Introduction
- Keys are always a String in redis
- Redis strings store sequences of bytes, including text, serialized objects, and binary arrays.
- As such, strings are the simplest type of value you can associate with a Redis key.
- Since Redis keys are strings, when we use the string type as a value too, we are mapping a string to another string.
- The string data type is useful for a number of use cases, like caching HTML fragments or pages.
- By default, a single Redis string can be a maximum of 512 MB.
- Most string operations are O(1), which means they're highly efficient. However, be careful with the SUBSTR, GETRANGE, and SETRANGE commands, which can be O(n). These random-access string commands may cause performance issues when dealing with large strings.

# Commands
- [SET - Write key (String) value (String) pair to redis cache](SET.ipynb)
- [MSET - Set multple String values for String key](MSET.ipynb)
- [MSETNX - Sets the given keys to their respective values. MSETNX will not perform any operation at all even if just a single key already exists](MSETNX.ipynb)
- [GET - Get the value of key](GET.ipynb)
- [MGET - Returns the values of all specified keys](MGET.ipynb)
- [Implement counters in redis cache using INCR, INCRBY, DECR, DECRBY](Strings_as_counters.ipynb)
- [SETRANGE - Update key in redis](SETRANGE.ipynb)
- [GETRANGE - Get substring of key in redis](GETRANGE.ipynb)