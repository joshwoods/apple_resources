

- Swift
- UnkeyedEncodingContainer
-  encodeConditional(\_:) 

Instance Method

# encodeConditional(\_:)

Encodes a reference to the given object only if it is encoded unconditionally elsewhere in the payload (previously, or in the future).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func encodeConditional(_ object: T) throws where T : AnyObject, T : Encodable
```

**Required** Default implementation provided.

## Parameters 

`object`  

The object to encode.

## Discussion

For encoders which don’t support this feature, the default implementation encodes the given object unconditionally.

For formats which don’t support this feature, the default implementation encodes the given object unconditionally.

Throws

`EncodingError.invalidValue` if the given value is invalid in the current context for this format.

## Default Implementations

### UnkeyedEncodingContainer Implementations

func encodeConditional&lt;T>(T) throws

Encodes a reference to the given object only if it is encoded unconditionally elsewhere in the payload (previously, or in the future).

