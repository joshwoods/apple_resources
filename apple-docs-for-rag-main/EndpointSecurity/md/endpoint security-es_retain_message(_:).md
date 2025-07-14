

- Endpoint Security
-  es_retain_message(\_:) 

Function

# es_retain_message(\_:)

Retains the given message, extending its lifetime until released.

macOS 11.0+

``` source
func es_retain_message(_ msg: UnsafePointer)
```

## Parameters 

`msg`  

The message to retain.

## Discussion

If you asynchronously process the message provided to the event-handler block of es_new_client(_:_:), you must retain the message.

## See Also

### Retaining and Releasing Messages

func es_release_message(UnsafePointer&lt;es_message_t>)

Releases a previously-retained message.

