

- SwiftUI
- DragGesture
-  minimumDistance 

Instance Property

# minimumDistance

The minimum dragging distance before the gesture succeeds.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
var minimumDistance: CGFloat
```

## See Also

### Creating a drag gesture

init(minimumDistance: CGFloat, coordinateSpace: some CoordinateSpaceProtocol)

Creates a dragging gesture with the minimum dragging distance before the gesture succeeds and the coordinate space of the gesture’s location.

var coordinateSpace: CoordinateSpace

The coordinate space in which to receive location values.

