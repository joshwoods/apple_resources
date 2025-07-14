

- Core Graphics
- CGContext
-  concatenate(\_:) 

Instance Method

# concatenate(\_:)

Transforms the user coordinate system in a context using a specified matrix.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func concatenate(_ transform: CGAffineTransform)
```

## Parameters 

`transform`  

The transformation matrix to apply to the specified context’s current transformation matrix.

## Discussion

When you call this function, it concatenates (that is, it combines) two matrices, by multiplying them together. The order in which matrices are concatenated is important, as the operations are not commutative. The resulting CTM in the context is: `CTMnew = transform * CTMcontext.`

## See Also

### Working with the Current Transformation Matrix

var ctm: CGAffineTransform

Returns the current transformation matrix.

func rotate(by: CGFloat)

Rotates the user coordinate system in a context.

func scaleBy(x: CGFloat, y: CGFloat)

Changes the scale of the user coordinate system in a context.

func translateBy(x: CGFloat, y: CGFloat)

Changes the origin of the user coordinate system in a context.

