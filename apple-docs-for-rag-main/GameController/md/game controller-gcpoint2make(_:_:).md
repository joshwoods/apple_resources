

- Game Controller
-  GCPoint2Make(\_:\_:) 

Function

# GCPoint2Make(\_:\_:)

Returns a point with the specified coordinates in a two-dimensional coordinate system.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.3+tvOS 17.4+visionOS 1.1+

``` source
func GCPoint2Make(
    _ x: Float,
    _ y: Float
) -> GCPoint2
```

## Parameters 

`x`  

The x-coordinate of the point.

`y`  

The y-coordinate of the point.

## Return Value

A point in a two-dimensional coordinate system.

## See Also

### Creating a point

init()

Creates a two dimensional point with coordinates `(0, 0)`.

init(x: Float, y: Float)

Creates a two dimensional point with the given coordinates.

let GCPoint2Zero: GCPoint2

The origin for a two dimensional point.

