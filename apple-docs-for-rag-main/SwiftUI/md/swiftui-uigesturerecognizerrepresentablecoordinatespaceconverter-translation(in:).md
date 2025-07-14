

- SwiftUI
- UIGestureRecognizerRepresentableCoordinateSpaceConverter
-  translation(in:) 

Instance Method

# translation(in:)

Converts the represented gesture recognizer’s current translation to a SwiftUI coordinate space of an ancestor of the view the gesture recognizer is attached to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
func translation(in coordinateSpace: some CoordinateSpaceProtocol) -> CGPoint?
```

## Parameters 

`coordinateSpace`  

The SwiftUI coordinate space to convert to.

## Discussion

If the gesture recognizer does not implement a `velocityInView:` method, returns nil.

