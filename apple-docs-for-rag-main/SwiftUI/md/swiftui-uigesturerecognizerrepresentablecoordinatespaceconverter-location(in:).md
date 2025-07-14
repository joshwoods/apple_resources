

- SwiftUI
- UIGestureRecognizerRepresentableCoordinateSpaceConverter
-  location(in:) 

Instance Method

# location(in:)

Converts the represented gesture recognizer’s current location to a SwiftUI coordinate space of an ancestor of the view the gesture recognizer is attached to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
func location(in coordinateSpace: some CoordinateSpaceProtocol) -> CGPoint
```

## Parameters 

`coordinateSpace`  

The SwiftUI coordinate space to convert to.

