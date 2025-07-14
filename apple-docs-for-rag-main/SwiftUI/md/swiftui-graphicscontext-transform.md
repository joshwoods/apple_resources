

- SwiftUI
- GraphicsContext
-  transform 

Instance Property

# transform

The current transform matrix, defining user space coordinates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var transform: CGAffineTransform { get set }
```

## Discussion

Modify this matrix to transform content that you subsequently draw into the context. Changes that you make don’t affect existing content.

## See Also

### Applying transforms

func scaleBy(x: CGFloat, y: CGFloat)

Scales subsequent drawing operations by an amount in each dimension.

func rotate(by: Angle)

Rotates subsequent drawing operations by an angle.

func translateBy(x: CGFloat, y: CGFloat)

Moves subsequent drawing operations by an amount in each dimension.

func concatenate(CGAffineTransform)

Appends the given transform to the context’s existing transform.

