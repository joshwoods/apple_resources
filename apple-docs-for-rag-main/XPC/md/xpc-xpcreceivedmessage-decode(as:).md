

- XPC
- XPCReceivedMessage
-  decode(as:) 

Instance Method

# decode(as:)

Decodes a message as the given type.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func decode(as type: T.Type = T.self) throws -> T where T : Decodable
```

## Parameters 

`type`  

The type of the value in the message.

## Return Value

A value of the specified type if the message data decodes successfully.

## Discussion

If the message data doesn’t decode to the type, this method throws the appropriate DecodingError.

## See Also

### Accessing message content

var isSync: Bool

A Boolean value that indicates if this message is from a synchronous request.

