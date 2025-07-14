

- SwiftUI
- GraphicsContext
-  translateBy(x:y:) 

Instance Method

# translateBy(x:y:)

Moves subsequent drawing operations by an amount in each dimension.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func translateBy(
    x: CGFloat,
    y: CGFloat
)
```

## Parameters 

`x`  

The amount to move in the horizontal direction.

`y`  

The amount to move in the vertical direction.

## Discussion

Calling this method is equivalent to updating the context’s transform directly using the given translation amount:

```
transform = transform.translatedBy(x: x, y: y)
```

## See Also

### Applying transforms

func scaleBy(x: CGFloat, y: CGFloat)

Scales subsequent drawing operations by an amount in each dimension.

func rotate(by: Angle)

Rotates subsequent drawing operations by an angle.

func concatenate(CGAffineTransform)

Appends the given transform to the context’s existing transform.

var transform: CGAffineTransform

The current transform matrix, defining user space coordinates.

