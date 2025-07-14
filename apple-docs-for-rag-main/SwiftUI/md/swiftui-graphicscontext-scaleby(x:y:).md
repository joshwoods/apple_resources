

- SwiftUI
- GraphicsContext
-  scaleBy(x:y:) 

Instance Method

# scaleBy(x:y:)

Scales subsequent drawing operations by an amount in each dimension.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func scaleBy(
    x: CGFloat,
    y: CGFloat
)
```

## Parameters 

`x`  

The amount to scale in the horizontal direction.

`y`  

The amount to scale in the vertical direction.

## Discussion

Calling this method is equivalent to updating the context’s transform directly using the given scale factors:

```
transform = transform.scaledBy(x: x, y: y)
```

## See Also

### Applying transforms

func rotate(by: Angle)

Rotates subsequent drawing operations by an angle.

func translateBy(x: CGFloat, y: CGFloat)

Moves subsequent drawing operations by an amount in each dimension.

func concatenate(CGAffineTransform)

Appends the given transform to the context’s existing transform.

var transform: CGAffineTransform

The current transform matrix, defining user space coordinates.

