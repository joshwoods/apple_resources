

- SwiftUI
- Path
-  contains(\_:eoFill:) 

Instance Method

# contains(\_:eoFill:)

Returns true if the path contains a specified point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func contains(
    _ p: CGPoint,
    eoFill: Bool = false
) -> Bool
```

## Discussion

If `eoFill` is true, this method uses the even-odd rule to define which points are inside the path. Otherwise, it uses the non-zero rule.

## See Also

### Getting the path’s characteristics

var boundingRect: CGRect

A rectangle containing all path segments.

var cgPath: CGPath

An immutable path representing the elements in the path.

var currentPoint: CGPoint?

Returns the last point in the path, or nil if the path contains no points.

var description: String

A description of the path that may be used to recreate the path via `init?(_:)`.

var isEmpty: Bool

A Boolean value indicating whether the path contains zero elements.

