

- SwiftUI
- SpatialTapGesture
-  count 

Instance Property

# count

The required number of tap events.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var count: Int
```

## See Also

### Creating a spatial tap gesture

init(count: Int, coordinateSpace: some CoordinateSpaceProtocol)

Creates a tap gesture with the number of required taps and the coordinate space of the gesture’s location.

var coordinateSpace: CoordinateSpace

The coordinate space in which to receive location values.

