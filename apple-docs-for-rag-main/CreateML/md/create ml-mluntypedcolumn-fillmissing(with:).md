

- Create ML
- MLUntypedColumn
-  fillMissing(with:) 

Instance Method

# fillMissing(with:)

Creates a modified copy of the column such that every missing element is replaced with the given value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func fillMissing(with value: MLDataValue) -> MLUntypedColumn
```

## Parameters 

`value`  

A value to replace every undefined element.

## Return Value

A new `MLDataColumn` column.

