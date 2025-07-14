

- TabularData
- Column
-  encoded(using:) 

Instance Method

# encoded(using:)

Generates a column by encoding each element’s value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func encoded(using encoder: Encoder) throws -> Column where Encoder : TopLevelEncoder
```

Available when `WrappedElement` conforms to `Encodable`.

## Parameters 

`encoder`  

An encoder.

## Return Value

A new column of encoded values.

## Discussion

Throws

`ColumnEncodingError` when the encoder fails to encode an element.

