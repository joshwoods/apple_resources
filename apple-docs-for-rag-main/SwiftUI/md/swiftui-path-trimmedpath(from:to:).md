

- SwiftUI
- Path
-  trimmedPath(from:to:) 

Instance Method

# trimmedPath(from:to:)

Returns a partial copy of the path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func trimmedPath(
    from: CGFloat,
    to: CGFloat
) -> Path
```

## Discussion

The returned path contains the region between `from` and `to`, both of which must be fractions between zero and one defining points linearly-interpolated along the path.

## See Also

### Transforming the path

func applying(CGAffineTransform) -> Path

Returns a path constructed by applying the transform to all points of the path.

func offsetBy(dx: CGFloat, dy: CGFloat) -> Path

Returns a path constructed by translating all its points.

