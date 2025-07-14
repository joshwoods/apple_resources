

- SwiftUI
- GraphicsContext
-  concatenate(\_:) 

Instance Method

# concatenate(\_:)

Appends the given transform to the context’s existing transform.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func concatenate(_ matrix: CGAffineTransform)
```

## Parameters 

`matrix`  

A transform to append to the existing transform.

## Discussion

Calling this method is equivalent to updating the context’s transform directly using the `matrix` parameter:

```
transform = matrix.concatenating(transform)
```

## See Also

### Applying transforms

func scaleBy(x: CGFloat, y: CGFloat)

Scales subsequent drawing operations by an amount in each dimension.

func rotate(by: Angle)

Rotates subsequent drawing operations by an angle.

func translateBy(x: CGFloat, y: CGFloat)

Moves subsequent drawing operations by an amount in each dimension.

var transform: CGAffineTransform

The current transform matrix, defining user space coordinates.

