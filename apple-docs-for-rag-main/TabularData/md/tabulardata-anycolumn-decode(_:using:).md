

- TabularData
- AnyColumn
-  decode(\_:using:) 

Instance Method

# decode(\_:using:)

Decodes the data in each element of the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func decode(
    _ type: T.Type,
    using decoder: Decoder
) throws where T : Decodable, Decoder : TopLevelDecoder
```

## Parameters 

`type`  

The type of the value to decode.

`decoder`  

A decoder that accepts the column elements’ type.

## Discussion

Throws

`ColumnDecodingError` if an element fails to decode.

## See Also

### Decoding a Column

func decoded&lt;T, Decoder>(T.Type, using: Decoder) throws -> AnyColumn

Decodes data for each element of the column.

