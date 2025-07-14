

- Swift
- RangeSet
- RangeSet.Ranges
-  RangeSet.Ranges.Index 

Type Alias

# RangeSet.Ranges.Index

A type that represents a position in the collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
typealias Index = Int
```

Available when `Bound` conforms to `Comparable`.

## Discussion

Valid indices consist of the position of every element and a “past the end” position that’s not valid for use as a subscript argument.

