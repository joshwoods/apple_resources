

- SwiftUI
- Path
-  description 

Instance Property

# description

A description of the path that may be used to recreate the path via `init?(_:)`.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var description: String { get }
```

## See Also

### Getting the path’s characteristics

var boundingRect: CGRect

A rectangle containing all path segments.

var cgPath: CGPath

An immutable path representing the elements in the path.

func contains(CGPoint, eoFill: Bool) -> Bool

Returns true if the path contains a specified point.

var currentPoint: CGPoint?

Returns the last point in the path, or nil if the path contains no points.

var isEmpty: Bool

A Boolean value indicating whether the path contains zero elements.

