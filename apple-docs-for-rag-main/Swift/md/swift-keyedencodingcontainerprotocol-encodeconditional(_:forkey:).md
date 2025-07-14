

- Swift
- KeyedEncodingContainerProtocol
-  encodeConditional(\_:forKey:) 

Instance Method

# encodeConditional(\_:forKey:)

Encodes a reference to the given object only if it is encoded unconditionally elsewhere in the payload (previously, or in the future).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func encodeConditional(
    _ object: T,
    forKey key: Self.Key
) throws where T : AnyObject, T : Encodable
```

**Required** Default implementation provided.

## Parameters 

`object`  

The object to encode.

`key`  

The key to associate the object with.

## Discussion

For encoders which don’t support this feature, the default implementation encodes the given object unconditionally.

Throws

`EncodingError.invalidValue` if the given value is invalid in the current context for this format.

## Default Implementations

### KeyedEncodingContainerProtocol Implementations

func encodeConditional&lt;T>(T, forKey: Self.Key) throws

Encodes a reference to the given object only if it is encoded unconditionally elsewhere in the payload (previously, or in the future).

