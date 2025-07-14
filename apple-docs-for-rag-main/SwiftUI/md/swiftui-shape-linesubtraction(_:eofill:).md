

- SwiftUI
- Shape
-  lineSubtraction(\_:eoFill:) 

Instance Method

# lineSubtraction(\_:eoFill:)

Returns a new shape with a line from this shape that does not overlap the filled region of the given shape.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func lineSubtraction(
    _ other: T,
    eoFill: Bool = false
) -> some Shape where T : Shape
```

## Parameters 

`other`  

The shape to subtract.

`eoFill`  

Whether to use the even-odd rule for determining which areas to treat as the interior of the shapes (if true), or the non-zero rule (if false).

## Return Value

A new shape.

## Discussion

The line of the resulting shape is the line of this shape that does not overlap the filled region of `other`.

Intersected subpaths that are clipped create open subpaths. Closed subpaths that do not intersect `other` remain closed.

## See Also

### Performing operations on a shape

func intersection&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions common to both shapes.

func lineIntersection&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with a line from this shape that overlaps the filled regions of the given shape.

func subtracting&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions from this shape that are not in the given shape.

func symmetricDifference&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions either from this shape or the given shape, but not in both.

func union&lt;T>(T, eoFill: Bool) -> some Shape

Returns a new shape with filled regions in either this shape or the given shape.

