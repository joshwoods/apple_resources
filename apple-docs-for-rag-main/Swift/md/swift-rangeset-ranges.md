

- Swift
- RangeSet
-  ranges 

Instance Property

# ranges

A collection of the ranges that make up the range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var ranges: RangeSet.Ranges { get }
```

## Discussion

The ranges that you access by using `ranges` never overlap, are never empty, and are always in increasing order.

