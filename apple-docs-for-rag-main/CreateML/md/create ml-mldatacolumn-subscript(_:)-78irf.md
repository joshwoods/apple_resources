

- Create ML
- MLDataColumn
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Creates a subset of the column by masking its elements with a column of Booleans.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(mask: MLDataColumn) -> MLDataColumn { get }
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`mask`  

A Boolean column indicating whether elements should be kept (`true`) or removed (`false`) in the derived column.

## Return Value

A new column.

## See Also

### Masking elements to generate a column

subscript(MLUntypedColumn) -> MLDataColumn&lt;Element>

Returns a `MLDataColumn` containing only the elements for which the corresponding mask has a nonzero or non-default value.

