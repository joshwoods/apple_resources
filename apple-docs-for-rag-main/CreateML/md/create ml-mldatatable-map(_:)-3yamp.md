

- Create ML
- MLDataTable
-  map(\_:) 

Instance Method

# map(\_:)

Creates a new column, potentially with missing values, by applying a given thread-safe transform to every row in the data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func map(_ lazyTransform: @escaping (MLDataTable.Row) -> T?) -> MLDataColumn where T : MLDataValueConvertible
```

## Parameters 

`lazyTransform`  

A thread-safe row transformation function.

The implementation of your transform must accept a row from the data table and return an optional type that conforms to MLDataValueConvertible. If the transform returns `nil` for a given row, the corresponding element in the new column will have a missing value.

## Return Value

A new MLDataColumn.

## Discussion

This mapping function is the same as map(_:) with the exception that this version’s `lazyTransform` parameter returns an optional (`T?`). Use this version of `map()` to create empty values by returning `nil` from your `lazyTransform`.

## See Also

### Transforming rows to generate a data column

func map&lt;T>((MLDataTable.Row) -> T) -> MLDataColumn&lt;T>

Creates a new column by applying a given thread-safe transform to every row in the data table.

