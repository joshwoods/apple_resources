

- SwiftUI
- SpatialTapGesture
-  coordinateSpace 

Instance Property

# coordinateSpace

The coordinate space in which to receive location values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var coordinateSpace: CoordinateSpace
```

## See Also

### Creating a spatial tap gesture

init(count: Int, coordinateSpace: some CoordinateSpaceProtocol)

Creates a tap gesture with the number of required taps and the coordinate space of the gesture’s location.

var count: Int

The required number of tap events.

