

- Create ML
- MLDataColumn
-  dropMissing() 

Instance Method

# dropMissing()

Creates a subset of the column by removing all elements without a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func dropMissing() -> MLDataColumn
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Return Value

A new column.

## See Also

### Discarding elements to generate a column

func dropDuplicates() -> MLDataColumn&lt;Element>

Creates a subset of the column by removing all duplicate elements.

