

- RealityKit
- NetworkCompatibilityToken
-  encode(to:) 

Instance Method

# encode(to:)

Writes the token’s data into an encoder.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS

``` source
final func encode(to encoder: any Encoder) throws
```

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

If the value fails to encode anything, `encoder` will encode an empty keyed container. This function throws an Error if any values are invalid for the given encoder’s format.

## See Also

### Serializing tokens

init(from: any Decoder) throws

Creates a new instance from a decoder.

