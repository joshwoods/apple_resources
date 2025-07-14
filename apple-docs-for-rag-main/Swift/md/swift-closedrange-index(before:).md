

- Swift
- ClosedRange
-  index(before:) 

Instance Method

# index(before:)

Returns the position immediately before the given index.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(before i: ClosedRange.Index) -> ClosedRange.Index
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

## Parameters 

`i`  

A valid index of the collection. `i` must be greater than `startIndex`.

## Return Value

The index value immediately before `i`.

