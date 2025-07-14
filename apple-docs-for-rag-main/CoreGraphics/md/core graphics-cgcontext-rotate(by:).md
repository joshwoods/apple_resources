

- Core Graphics
- CGContext
-  rotate(by:) 

Instance Method

# rotate(by:)

Rotates the user coordinate system in a context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func rotate(by angle: CGFloat)
```

## Parameters 

`angle`  

The angle, in radians, by which to rotate the coordinate space of the specified context. Positive values rotate counterclockwise and negative values rotate clockwise.)

## Discussion

The direction that the context is rotated may appear to be altered by the state of the current transformation matrix prior to executing this function. For example, on iOS, a UIView applies a transformation to the graphics context that inverts the Y-axis (by multiplying it by `-1`). Rotating the user coordinate system on coordinate system that was previously flipped results in a rotation in the opposite direction (that is, positive values appear to rotate the coordinate system in the clockwise direction).

## See Also

### Working with the Current Transformation Matrix

var ctm: CGAffineTransform

Returns the current transformation matrix.

func scaleBy(x: CGFloat, y: CGFloat)

Changes the scale of the user coordinate system in a context.

func translateBy(x: CGFloat, y: CGFloat)

Changes the origin of the user coordinate system in a context.

func concatenate(CGAffineTransform)

Transforms the user coordinate system in a context using a specified matrix.

