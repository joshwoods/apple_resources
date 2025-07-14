

- Swift
- RangeSet
-  init(\_:) 

Initializer

# init(\_:)

Creates a range set containing the values in the given ranges.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(_ ranges: some Sequence>)
```

## Parameters 

`ranges`  

The ranges to use for the new range set.

## Discussion

Any empty ranges in `ranges` are ignored, and non-empty ranges are merged to eliminate any overlaps. As such, the `ranges` collection in the resulting range set may not be equivalent to the sequence of ranges passed to this initializer.

