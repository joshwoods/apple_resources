

- SwiftUI
-  UIGestureRecognizerRepresentableCoordinateSpaceConverter 

Structure

# UIGestureRecognizerRepresentableCoordinateSpaceConverter

A proxy structure used to convert locations to/from coordinate spaces in the hierarchy of the SwiftUI view associated with a UIGestureRecognizerRepresentable.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
struct UIGestureRecognizerRepresentableCoordinateSpaceConverter
```

## Topics

### Instance Properties

var localLocation: CGPoint

The represented gesture recognizer’s current location in the coordinate space of the SwiftUI view it’s attached to.

var localTranslation: CGPoint?

The represented gesture recognizer’s current translation in the coordinate space of the SwiftUI view it’s attached to.

var localVelocity: CGPoint?

The represented gesture recognizer’s current velocity in the coordinate space of the SwiftUI view it’s attached to.

### Instance Methods

func convert(globalPoint: CGPoint, to: some CoordinateSpaceProtocol) -> CGPoint

Converts a point in the global coordinate space to a SwiftUI coordinate space of an ancestor of the view the gesture recognizer is attached to.

func location(in: some CoordinateSpaceProtocol) -> CGPoint

Converts the represented gesture recognizer’s current location to a SwiftUI coordinate space of an ancestor of the view the gesture recognizer is attached to.

func translation(in: some CoordinateSpaceProtocol) -> CGPoint?

Converts the represented gesture recognizer’s current translation to a SwiftUI coordinate space of an ancestor of the view the gesture recognizer is attached to.

func velocity(in: some CoordinateSpaceProtocol) -> CGPoint?

Converts the represented gesture recognizer’s current velocity to a SwiftUI coordinate space of an ancestor of the view the gesture recognizer is attached to.

## See Also

### Integrate gesture recognizer into SwiftUI view hierarchies

protocol UIGestureRecognizerRepresentable

A wrapper for a `UIGestureRecognizer` that you use to integrate that gesture recognizer into your SwiftUI hierarchy.

struct UIGestureRecognizerRepresentableContext

Contextual information about the state of the system that you use to create and update a represented gesture recognizer.

