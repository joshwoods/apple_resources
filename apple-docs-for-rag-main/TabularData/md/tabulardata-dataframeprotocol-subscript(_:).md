

- TabularData
- DataFrameProtocol
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a slice of the data frame type with an index range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(range: Range) -> DataFrame.Slice { get set }
```

**Required** Default implementations provided.

## Parameters 

`range`  

An integer range.

## Default Implementations

### DataFrameProtocol Implementations

subscript&lt;R>(R) -> DataFrame.Slice

Accesses rows of a data frame type with an index range expression.

subscript(Range&lt;Int>) -> DataFrame.Slice

Accesses a slice of the data frame type with an index range.

## See Also

### Accessing Rows

subscript&lt;R>(R) -> DataFrame.Slice

Accesses rows of a data frame type with an index range expression.

