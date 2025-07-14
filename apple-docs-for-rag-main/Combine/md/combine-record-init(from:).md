

- Combine
- Record
-  init(from:) 

Initializer

# init(from:)

Creates a new instance by decoding from the given decoder.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(from decoder: any Decoder) throws
```

Available when `Output` conforms to `Decodable`, `Output` conforms to `Encodable`, `Failure` conforms to `Decodable`, `Failure` conforms to `Encodable`, and `Failure` conforms to `Error`.

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

