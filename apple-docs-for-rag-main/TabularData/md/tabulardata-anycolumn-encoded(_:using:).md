

- TabularData
- AnyColumn
-  encoded(\_:using:) 

Instance Method

# encoded(\_:using:)

Generates a column by encoding each element’s value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func encoded(
    _ type: T.Type,
    using encoder: Encoder
) throws -> AnyColumn where T : Encodable, Encoder : TopLevelEncoder
```

## Parameters 

`type`  

The column underlying type.

`encoder`  

An encoder.

## Return Value

A new column of encoded values.

## Discussion

Throws

`ColumnEncodingError` when the encoder fails to encode an element.

## See Also

### Encoding a Column

func encode&lt;T, Encoder>(T.Type, using: Encoder) throws

Encodes each element of the column.

