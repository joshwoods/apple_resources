

- Create ML
- MLDataColumn
-  dropDuplicates() 

Instance Method

# dropDuplicates()

Creates a subset of the column by removing all duplicate elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func dropDuplicates() -> MLDataColumn
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Return Value

A new column.

## Discussion

Note

The new column may not preserve the order of the original column.

## See Also

### Discarding elements to generate a column

func dropMissing() -> MLDataColumn&lt;Element>

Creates a subset of the column by removing all elements without a value.

