

- Core Graphics
- CGContext
-  draw(\_:at:) 

Instance Method

# draw(\_:at:)

Draws the contents of a layer object at the specified point.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func draw(
    _ layer: CGLayer,
    at point: CGPoint
)
```

## Parameters 

`layer`  

The layer whose contents you want to draw.

`point`  

The location, in current user space coordinates, to use as the origin for the drawing.

## Discussion

Calling this method is equivalent to calling the draw(_:in:) method with a rectangle whose origin is the specified point and whose size matches that of the specified layer.

## See Also

### Drawing Core Graphics Layers

func draw(CGLayer, in: CGRect)

Draws the contents of a layer object into the specified rectangle.

