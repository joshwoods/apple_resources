

- Endpoint Security
-  es_string_token_t 

Structure

# es_string_token_t

A pointer to a null-terminated string, and the length in bytes of that string.

Mac CatalystmacOS

``` source
struct es_string_token_t
```

## Overview

The length doesn’t include the null terminator character.

## Topics

### Initializers

init()

init(length: Int, data: UnsafePointer&lt;CChar>!)

### Inspecting the Token

var data: UnsafePointer&lt;CChar>!

The string data.

var length: Int

The size of the data buffer, in bytes.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Supporting Types

struct es_result_t

The result of the Endpoint Security subsystem authorization process.

struct es_token_t

An arbitrary buffer of data with its size.

