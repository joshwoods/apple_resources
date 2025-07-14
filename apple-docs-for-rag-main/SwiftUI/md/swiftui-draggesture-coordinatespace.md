

- SwiftUI
- DragGesture
-  coordinateSpace 

Instance Property

# coordinateSpace

The coordinate space in which to receive location values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
var coordinateSpace: CoordinateSpace
```

## See Also

### Creating a drag gesture

init(minimumDistance: CGFloat, coordinateSpace: some CoordinateSpaceProtocol)

Creates a dragging gesture with the minimum dragging distance before the gesture succeeds and the coordinate space of the gesture’s location.

var minimumDistance: CGFloat

The minimum dragging distance before the gesture succeeds.

