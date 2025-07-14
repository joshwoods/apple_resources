

- Swift
- Dictionary
-  init(from:) 

Initializer

# init(from:)

Creates a new dictionary by decoding from the given decoder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(from decoder: any Decoder) throws
```

Available when `Key` conforms to `Decodable`, `Key` conforms to `Hashable`, and `Value` conforms to `Decodable`.

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

## See Also

### Encoding and Decoding

func encode(to: any Encoder) throws

Encodes the contents of this dictionary into the given encoder.

