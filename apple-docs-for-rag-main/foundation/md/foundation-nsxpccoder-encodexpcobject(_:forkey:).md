

- Foundation
- NSXPCCoder
-  encodeXPCObject(\_:forKey:) 

Instance Method

# encodeXPCObject(\_:forKey:)

Encodes an object to send over an XPC connection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+

``` source
func encodeXPCObject(
    _ xpcObject: xpc_object_t,
    forKey key: String
)
```

## Parameters 

`xpcObject`  

An object that XPC can encode.

`key`  

A string that your app uses to reference the encoded object.

## See Also

### Encoding and Decoding

func decodeXPCObject(ofType: xpc_type_t, forKey: String) -> xpc_object_t?

Decodes an object and validates that its type matches the type a service provides over XPC.

