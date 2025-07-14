

- Create ML
- MLUntypedColumn
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Creates a subset of the column, given a range expression of elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(slice: R) -> MLUntypedColumn where R : RangeExpression, R.Bound == Int { get }
```

## Parameters 

`slice`  

An interger range expression indicating which elements to include in the new column.

## Return Value

A new column.

## See Also

### Selecting elements to generate an untyped column

subscript(Range&lt;Int>) -> MLUntypedColumn

Creates a subset of the column, given a range of elements.

func prefix(Int) -> MLUntypedColumn

Creates a subset of the column, given a number of initial elements.

func suffix(Int) -> MLUntypedColumn

Creates a subset of the column, given a number of final elements.

