

- SwiftUI
- Shape
-  intersection(\_:eoFill:) 

Instance Method

# intersection(\_:eoFill:)

Returns a new shape with filled regions common to both shapes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func intersection(
    _ other: T,
    eoFill: Bool = false
) -> some Shape where T : Shape
```

## Parameters 

`other`  

The shape to intersect.

`eoFill`  

Whether to use the even-odd rule for determining which areas to treat as the interior of the shapes (if true), or the non-zero rule (if false).

## Return Value

A new shape.

## Discussion

The filled region of the resulting shape is the overlapping area of the filled region of both shapes. This can be used to clip the fill of a shape to a mask.

Any unclosed subpaths in either shape are assumed to be closed. The result of filling this shape using either even-odd or non-zero fill rules is identical.

## See Also

### Performing operations on a shape

func lineIntersection&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with a line from this shape that overlaps the filled regions of the given shape.

func lineSubtraction&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with a line from this shape that does not overlap the filled region of the given shape.

func subtracting&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions from this shape that are not in the given shape.

func symmetricDifference&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions either from this shape or the given shape, but not in both.

func union&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions in either this shape or the given shape.

