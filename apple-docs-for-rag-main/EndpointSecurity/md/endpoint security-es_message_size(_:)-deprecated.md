

- Endpoint Security
-  es_message_size(\_:) Deprecated

Function

# es_message_size(\_:)

Calculates the size of a message structure.

iOS 18.0–18.0DeprecatediPadOS 18.0–18.0DeprecatedMac Catalyst 18.0–18.0DeprecatedmacOS 10.15–11.0Deprecated

``` source
func es_message_size(_ msg: UnsafePointer) -> Int
```

Deprecated

Use es_retain_message(_:) to retain a message. Don’t use es_message_size(_:) in conjunction with attempting to copy a message; doing so will result in use-after-free bugs.

## Parameters 

`msg`  

The message to calculate the size of.

## Return Value

The calculated size of the message.

## See Also

### Deprecated Functions

func es_copy_message(UnsafePointer&lt;es_message_t>) -> UnsafeMutablePointer&lt;es_message_t>?

Copies a message, by allocating new memory.

Deprecated

func es_free_message(UnsafeMutablePointer&lt;es_message_t>)

Frees the memory allocated for the given message.

Deprecated

