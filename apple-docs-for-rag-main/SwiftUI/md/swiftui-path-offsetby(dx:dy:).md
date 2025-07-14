

- SwiftUI
- Path
-  offsetBy(dx:dy:) 

Instance Method

# offsetBy(dx:dy:)

Returns a path constructed by translating all its points.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func offsetBy(
    dx: CGFloat,
    dy: CGFloat
) -> Path
```

## Parameters 

`dx`  

The offset to apply in the horizontal axis.

`dy`  

The offset to apply in the vertical axis.

## Return Value

A new copy of the path with the offset applied to all points.

## See Also

### Transforming the path

func applying(CGAffineTransform) -> Path

Returns a path constructed by applying the transform to all points of the path.

func trimmedPath(from: CGFloat, to: CGFloat) -> Path

Returns a partial copy of the path.

