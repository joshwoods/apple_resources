

- SwiftUI
- SpatialTapGesture
-  init(count:coordinateSpace:) 

Initializer

# init(count:coordinateSpace:)

Creates a tap gesture with the number of required taps and the coordinate space of the gesture’s location.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    count: Int = 1,
    coordinateSpace: some CoordinateSpaceProtocol = .local
)
```

Show all declarations

## Parameters 

`count`  

The required number of taps to complete the tap gesture.

`coordinateSpace`  

The coordinate space of the tap gesture’s location.

