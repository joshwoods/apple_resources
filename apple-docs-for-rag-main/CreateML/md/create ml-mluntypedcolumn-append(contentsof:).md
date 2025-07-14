

- Create ML
- MLUntypedColumn
-  append(contentsOf:) 

Instance Method

# append(contentsOf:)

Appends the elements of the given column to the end of this column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
mutating func append(contentsOf newColumn: MLUntypedColumn)
```

## Parameters 

`newColumn`  

Another column to append to the column.

## Discussion

Note

The type of `newColumn` must be the same type or convertible to the same type as this column. See MLDataValueConvertible.

