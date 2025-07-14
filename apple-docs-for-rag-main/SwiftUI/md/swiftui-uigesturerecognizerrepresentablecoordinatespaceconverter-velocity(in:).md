

- SwiftUI
- UIGestureRecognizerRepresentableCoordinateSpaceConverter
-  velocity(in:) 

Instance Method

# velocity(in:)

Converts the represented gesture recognizer’s current velocity to a SwiftUI coordinate space of an ancestor of the view the gesture recognizer is attached to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
func velocity(in coordinateSpace: some CoordinateSpaceProtocol) -> CGPoint?
```

## Parameters 

`coordinateSpace`  

The SwiftUI coordinate space to convert to.

## Discussion

If the gesture recognizer does not implement a `velocityInView:` method, returns nil.

