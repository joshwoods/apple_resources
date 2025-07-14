

- Endpoint Security
-  es_copy_message(\_:) Deprecated

Function

# es_copy_message(\_:)

Copies a message, by allocating new memory.

macOS 10.15–11.0Deprecated

``` source
func es_copy_message(_ msg: UnsafePointer) -> UnsafeMutablePointer?
```

Deprecated

Use es_retain_message(_:) to retain a message.

## Parameters 

`msg`  

The message to copy.

## Return Value

A pointer to a copy of the original message.

## Discussion

After calling this function, the caller owns this memory and must eventually free it with es_free_message(_:) to avoid leaking memory.

## See Also

### Deprecated Functions

func es_message_size(UnsafePointer&lt;es_message_t>) -> Int

Calculates the size of a message structure.

Deprecated

func es_free_message(UnsafeMutablePointer&lt;es_message_t>)

Frees the memory allocated for the given message.

Deprecated

