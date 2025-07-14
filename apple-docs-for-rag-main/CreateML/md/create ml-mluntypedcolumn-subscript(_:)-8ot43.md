

- Create ML
- MLUntypedColumn
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Creates a subset of the column by masking its elements with a data column of Booleans.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(mask: MLDataColumn) -> MLUntypedColumn { get }
```

## Parameters 

`mask`  

A Boolean column indicating whether elements should be kept (`true`) or removed (`false`) in the derived column.

## Return Value

A new column.

## See Also

### Masking elements to generate an untyped column

subscript(MLUntypedColumn) -> MLUntypedColumn

Creates a subset of the column by masking its elements with another untyped column.

