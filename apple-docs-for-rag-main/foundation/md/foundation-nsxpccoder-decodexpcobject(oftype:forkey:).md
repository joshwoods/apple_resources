

- Foundation
- NSXPCCoder
-  decodeXPCObject(ofType:forKey:) 

Instance Method

# decodeXPCObject(ofType:forKey:)

Decodes an object and validates that its type matches the type a service provides over XPC.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+

``` source
func decodeXPCObject(
    ofType type: xpc_type_t,
    forKey key: String
) -> xpc_object_t?
```

## Parameters 

`type`  

An opaque pointer to an encoded XPC object.

`key`  

A string that your app uses to reference the decoded object.

## Return Value

An object that XPC can encode.

## Discussion

The decodeXPCObject(ofType:forKey:) method validates that the type of the decoded object matches the type of the encoded object. If they don’t match, the NSXPCCoder throws an exception in support of NSSecureCoding.

Be sure to check the result against null if you call an XPC function because calling an XPC function on a null object results in a crash.

## See Also

### Encoding and Decoding

func encodeXPCObject(xpc_object_t, forKey: String)

Encodes an object to send over an XPC connection.

