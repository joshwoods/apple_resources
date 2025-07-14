

- Create ML
- MLPhase
-  init(from:) 

Initializer

# init(from:)

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `String`.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(from decoder: any Decoder) throws
```

Available when `Self` conforms to `Decodable` and `RawValue` is `String`.

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

## See Also

### Encoding and decoding a phase

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `String`.

