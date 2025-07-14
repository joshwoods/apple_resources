

- Core Graphics
- CGContext
-  scaleBy(x:y:) 

Instance Method

# scaleBy(x:y:)

Changes the scale of the user coordinate system in a context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func scaleBy(
    x sx: CGFloat,
    y sy: CGFloat
)
```

## Parameters 

`sx`  

The factor by which to scale the x-axis of the coordinate space of the specified context.

`sy`  

The factor by which to scale the y-axis of the coordinate space of the specified context.

## See Also

### Working with the Current Transformation Matrix

var ctm: CGAffineTransform

Returns the current transformation matrix.

func rotate(by: CGFloat)

Rotates the user coordinate system in a context.

func translateBy(x: CGFloat, y: CGFloat)

Changes the origin of the user coordinate system in a context.

func concatenate(CGAffineTransform)

Transforms the user coordinate system in a context using a specified matrix.

