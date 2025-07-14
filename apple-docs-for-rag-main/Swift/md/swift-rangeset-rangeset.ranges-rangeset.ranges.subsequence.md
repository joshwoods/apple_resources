

- Swift
- RangeSet
- RangeSet.Ranges
-  RangeSet.Ranges.SubSequence 

Type Alias

# RangeSet.Ranges.SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
typealias SubSequence = Slice.Ranges>
```

Available when `Bound` conforms to `Comparable`.

## Discussion

The default subsequence type for collections that don’t define their own is `Slice`.

