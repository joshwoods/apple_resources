

- Core Graphics
- CGContext
-  translateBy(x:y:) 

Instance Method

# translateBy(x:y:)

Changes the origin of the user coordinate system in a context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func translateBy(
    x tx: CGFloat,
    y ty: CGFloat
)
```

## Parameters 

`tx`  

The amount to displace the x-axis of the coordinate space, in units of the user space, of the specified context.

`ty`  

The amount to displace the y-axis of the coordinate space, in units of the user space, of the specified context.

## See Also

### Working with the Current Transformation Matrix

var ctm: CGAffineTransform

Returns the current transformation matrix.

func rotate(by: CGFloat)

Rotates the user coordinate system in a context.

func scaleBy(x: CGFloat, y: CGFloat)

Changes the scale of the user coordinate system in a context.

func concatenate(CGAffineTransform)

Transforms the user coordinate system in a context using a specified matrix.

