

- Endpoint Security
-  es_token_t 

Structure

# es_token_t

An arbitrary buffer of data with its size.

Mac CatalystmacOS

``` source
struct es_token_t
```

## Topics

### Inspecting the Token

var data: UnsafePointer&lt;UInt8>!

A data buffer.

var size: Int

The size of the data buffer, in bytes.

### Initializers

init()

init(size: Int, data: UnsafePointer&lt;UInt8>!)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Supporting Types

struct es_result_t

The result of the Endpoint Security subsystem authorization process.

struct es_string_token_t

A pointer to a null-terminated string, and the length in bytes of that string.

