

- Create ML
- MLUntypedColumn
-  suffix(\_:) 

Instance Method

# suffix(\_:)

Creates a subset of the column, given a number of final elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func suffix(_ maxLength: Int = 10) -> MLUntypedColumn
```

## Parameters 

`maxLength`  

The largest number of elements to use from the end of the column. The default value is `10`.

## Return Value

A new column.

## See Also

### Selecting elements to generate an untyped column

subscript(Range&lt;Int>) -> MLUntypedColumn

Creates a subset of the column, given a range of elements.

subscript&lt;R>(R) -> MLUntypedColumn

Creates a subset of the column, given a range expression of elements.

func prefix(Int) -> MLUntypedColumn

Creates a subset of the column, given a number of initial elements.

