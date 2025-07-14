

- TabularData
- RowGrouping
-  RowGrouping.SubSequence 

Type Alias

# RowGrouping.SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias SubSequence = Slice>
```

Available when `GroupingKey` conforms to `Hashable`.

## Discussion

The default subsequence type for collections that don’t define their own is `Slice`.

