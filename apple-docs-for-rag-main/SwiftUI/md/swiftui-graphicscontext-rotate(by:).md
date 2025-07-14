

- SwiftUI
- GraphicsContext
-  rotate(by:) 

Instance Method

# rotate(by:)

Rotates subsequent drawing operations by an angle.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func rotate(by angle: Angle)
```

## Parameters 

`angle`  

The amount to rotate.

## Discussion

Calling this method is equivalent to updating the context’s transform directly using the `angle` parameter:

```
transform = transform.rotated(by: angle.radians)
```

## See Also

### Applying transforms

func scaleBy(x: CGFloat, y: CGFloat)

Scales subsequent drawing operations by an amount in each dimension.

func translateBy(x: CGFloat, y: CGFloat)

Moves subsequent drawing operations by an amount in each dimension.

func concatenate(CGAffineTransform)

Appends the given transform to the context’s existing transform.

var transform: CGAffineTransform

The current transform matrix, defining user space coordinates.

