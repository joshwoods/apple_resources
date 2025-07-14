

- Create ML
- MLDataColumn
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns a `MLDataColumn` containing only the elements for which the corresponding mask has a nonzero or non-default value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(mask: MLUntypedColumn) -> MLDataColumn { get }
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`mask`  

A MLUntypedColumn with the same element count as this MLUntypedColumn.

## Return Value

A MLUntypedColumn containing the subsequence of this MLUntypedColumn’s elements indicated by the mask MLUntypedColumn.

## See Also

### Masking elements to generate a column

subscript(MLDataColumn&lt;Bool>) -> MLDataColumn&lt;Element>

Creates a subset of the column by masking its elements with a column of Booleans.

