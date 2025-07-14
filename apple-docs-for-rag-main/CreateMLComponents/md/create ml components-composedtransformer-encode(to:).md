

- Create ML Components
- ComposedTransformer
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Inner` conforms to `Transformer`, `Inner` conforms to `Encodable`, `Outer` conforms to `Transformer`, `Outer` conforms to `Encodable`, and `Inner.Output` is `Outer.Input`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

If the value fails to encode anything, `encoder` will encode an empty keyed container in its place.

This function throws an error if any values are invalid for the given encoder’s format.

