

- Core Graphics
- CGContext
-  ctm 

Instance Property

# ctm

Returns the current transformation matrix.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var ctm: CGAffineTransform { get }
```

## See Also

### Working with the Current Transformation Matrix

func rotate(by: CGFloat)

Rotates the user coordinate system in a context.

func scaleBy(x: CGFloat, y: CGFloat)

Changes the scale of the user coordinate system in a context.

func translateBy(x: CGFloat, y: CGFloat)

Changes the origin of the user coordinate system in a context.

func concatenate(CGAffineTransform)

Transforms the user coordinate system in a context using a specified matrix.

