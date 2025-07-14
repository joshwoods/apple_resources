

- TabularData
- CategoricalSummary
-  someCount 

Instance Property

# someCount

The number of non-missing elements in the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var someCount: Int
```

## See Also

### Inspecting a Summary

var debugDescription: String

A text representation of the summary’s statistics suitable for debugging.

var mode: [Element]

The most common values in a column, ignoring missing elements.

var uniqueCount: Int

The number of elements with distinct values in a column that excludes missing elements.

var noneCount: Int

The number of missing elements in the column.

var totalCount: Int

The total number of elements in the column.

