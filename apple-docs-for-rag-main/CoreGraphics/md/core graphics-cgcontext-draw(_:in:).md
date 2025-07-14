

- Core Graphics
- CGContext
-  draw(\_:in:) 

Instance Method

# draw(\_:in:)

Draws the contents of a layer object into the specified rectangle.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func draw(
    _ layer: CGLayer,
    in rect: CGRect
)
```

## Parameters 

`layer`  

The layer whose contents you want to draw.

`rect`  

The rectangle, in current user space coordinates, to draw in.

## Discussion

The contents are scaled, if necessary, to fit into the rectangle.

## See Also

### Drawing Core Graphics Layers

func draw(CGLayer, at: CGPoint)

Draws the contents of a layer object at the specified point.

