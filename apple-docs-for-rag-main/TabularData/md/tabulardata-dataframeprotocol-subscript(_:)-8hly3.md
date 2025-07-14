

- TabularData
- DataFrameProtocol
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses rows of a data frame type with an index range expression.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(r: R) -> DataFrame.Slice where R : RangeExpression, R.Bound == Int { get set }
```

## Parameters 

`r`  

An integer range expression.

## See Also

### Accessing Rows

subscript(Range&lt;Int>) -> DataFrame.Slice

Accesses a slice of the data frame type with an index range.

**Required** Default implementations provided.

