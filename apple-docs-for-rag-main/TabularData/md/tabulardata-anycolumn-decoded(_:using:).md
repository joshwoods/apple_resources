

- TabularData
- AnyColumn
-  decoded(\_:using:) 

Instance Method

# decoded(\_:using:)

Decodes data for each element of the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func decoded(
    _ type: T.Type,
    using decoder: Decoder
) throws -> AnyColumn where T : Decodable, Decoder : TopLevelDecoder
```

## Parameters 

`type`  

The type of the value to decode.

`decoder`  

A decoder that accepts the column elements’ type.

## Return Value

A new column of decoded values.

## Discussion

Throws

`ColumnDecodingError` if an element fails to decode.

## See Also

### Decoding a Column

func decode&lt;T, Decoder>(T.Type, using: Decoder) throws

Decodes the data in each element of the column.

