

- SwiftUI
- UIGestureRecognizerRepresentableCoordinateSpaceConverter
-  localVelocity 

Instance Property

# localVelocity

The represented gesture recognizer’s current velocity in the coordinate space of the SwiftUI view it’s attached to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
var localVelocity: CGPoint? { get }
```

## Discussion

If the gesture recognizer does not implement a `velocityInView:` method, returns nil.

