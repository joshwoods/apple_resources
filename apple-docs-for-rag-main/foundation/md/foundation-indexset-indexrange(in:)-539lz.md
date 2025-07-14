

- Foundation
- IndexSet
-  indexRange(in:) 

Instance Method

# indexRange(in:)

Return a `Range` which can be used to subscript the index set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func indexRange(in range: Range) -> Range
```

## Parameters 

`range`  

The range of integers to include.

## Discussion

The resulting range is the range of the intersection of the integers in `range` with the index set. The resulting range will be `isEmpty` if the intersection is empty.

