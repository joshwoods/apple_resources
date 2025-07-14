

- TabularData
- AnyColumn
-  encode(\_:using:) 

Instance Method

# encode(\_:using:)

Encodes each element of the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func encode(
    _ type: T.Type,
    using encoder: Encoder
) throws where T : Encodable, Encoder : TopLevelEncoder
```

## Parameters 

`type`  

The type of elements in the column.

`encoder`  

An encoder.

## Discussion

Throws

`ColumnEncodingError` if an element fails to encode.

## See Also

### Encoding a Column

func encoded&lt;T, Encoder>(T.Type, using: Encoder) throws -> AnyColumn

Generates a column by encoding each element’s value.

