

- Endpoint Security
-  es_release_message(\_:) 

Function

# es_release_message(\_:)

Releases a previously-retained message.

macOS 11.0+

``` source
func es_release_message(_ msg: UnsafePointer)
```

## Parameters 

`msg`  

The message to release.

## See Also

### Retaining and Releasing Messages

func es_retain_message(UnsafePointer&lt;es_message_t>)

Retains the given message, extending its lifetime until released.

