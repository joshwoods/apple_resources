

- Swift
- Range
-  clamped(to:) 

Instance Method

# clamped(to:)

Returns a copy of this range clamped to the given limiting range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func clamped(to limits: Range) -> Range
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`limits`  

The range to clamp the bounds of this range.

## Return Value

A new range clamped to the bounds of `limits`.

## Discussion

The bounds of the result are always limited to the bounds of `limits`. For example:

```
let x: Range = 0..

If the two ranges do not overlap, the result is an empty range within the bounds of `limits`.

```
let y: Range = 0..

