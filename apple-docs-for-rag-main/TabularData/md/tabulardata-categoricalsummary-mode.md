

- TabularData
- CategoricalSummary
-  mode 

Instance Property

# mode

The most common values in a column, ignoring missing elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var mode: [Element]
```

## Discussion

The summary orders the elements based on their original locations within the column.

## See Also

### Inspecting a Summary

var debugDescription: String

A text representation of the summary’s statistics suitable for debugging.

var uniqueCount: Int

The number of elements with distinct values in a column that excludes missing elements.

var someCount: Int

The number of non-missing elements in the column.

var noneCount: Int

The number of missing elements in the column.

var totalCount: Int

The total number of elements in the column.

