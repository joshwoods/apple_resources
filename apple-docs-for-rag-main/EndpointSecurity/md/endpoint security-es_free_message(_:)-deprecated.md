

- Endpoint Security
-  es_free_message(\_:) Deprecated

Function

# es_free_message(\_:)

Frees the memory allocated for the given message.

macOS 10.15–11.0Deprecated

``` source
func es_free_message(_ msg: UnsafeMutablePointer)
```

Deprecated

Use es_release_message(_:) to release a message.

## Parameters 

`msg`  

The message to free.

## Discussion

Only free messages you explicitly copied with es_copy_message(_:).

Warning

Freeing a message from inside a handler block will cause your app to crash.

## See Also

### Deprecated Functions

func es_copy_message(UnsafePointer&lt;es_message_t>) -> UnsafeMutablePointer&lt;es_message_t>?

Copies a message, by allocating new memory.

Deprecated

func es_message_size(UnsafePointer&lt;es_message_t>) -> Int

Calculates the size of a message structure.

Deprecated

