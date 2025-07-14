

- Create ML
- MLDataColumn
-  isValid 

Instance Property

# isValid

A Boolean value that indicates whether the column is valid.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var isValid: Bool { get }
```

## Discussion

Check isValid after you create or mutate a data column to ensure it’s valid. If the value is false, the data column encountered an error and you can’t use it for subsequent operations. For example, comparing two columns of different sizes creates an invalid column.

## See Also

### Handling data column errors

var error: (any Error)?

The underlying error present when the column is invalid.

