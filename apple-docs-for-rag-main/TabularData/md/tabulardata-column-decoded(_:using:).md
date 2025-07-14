

- TabularData
- Column
-  decoded(\_:using:) 

Instance Method

# decoded(\_:using:)

Generates a column by decoding each element’s data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func decoded(
    _ type: T.Type,
    using decoder: Decoder
) throws -> Column where WrappedElement == Decoder.Input, T : Decodable, Decoder : TopLevelDecoder
```

## Parameters 

`type`  

The decodable value’s type.

`decoder`  

A decoder.

## Return Value

A new column of decoded values.

## Discussion

Throws

`ColumnDecodingError` when the decoder fails to decode an element.

