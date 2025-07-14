

- SwiftUI
- Path
-  applying(\_:) 

Instance Method

# applying(\_:)

Returns a path constructed by applying the transform to all points of the path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func applying(_ transform: CGAffineTransform) -> Path
```

## Parameters 

`transform`  

An affine transform to apply to the path.

## Return Value

A new copy of the path with the transform applied to all points.

## See Also

### Transforming the path

func offsetBy(dx: CGFloat, dy: CGFloat) -> Path

Returns a path constructed by translating all its points.

func trimmedPath(from: CGFloat, to: CGFloat) -> Path

Returns a partial copy of the path.

