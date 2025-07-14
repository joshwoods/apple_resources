

- SwiftUI
- UIGestureRecognizerRepresentableCoordinateSpaceConverter
-  convert(globalPoint:to:) 

Instance Method

# convert(globalPoint:to:)

Converts a point in the global coordinate space to a SwiftUI coordinate space of an ancestor of the view the gesture recognizer is attached to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
func convert(
    globalPoint: CGPoint,
    to coordinateSpace: some CoordinateSpaceProtocol = .local
) -> CGPoint
```

## Parameters 

`globalPoint`  

The point in the global coordinate space.

`coordinateSpace`  

The SwiftUI coordinate space to convert to.

