

- SwiftUI
-  UIGestureRecognizerRepresentableContext 

Structure

# UIGestureRecognizerRepresentableContext

Contextual information about the state of the system that you use to create and update a represented gesture recognizer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
struct UIGestureRecognizerRepresentableContext where Representable : UIGestureRecognizerRepresentable
```

## Topics

### Instance Properties

let converter: UIGestureRecognizerRepresentableCoordinateSpaceConverter

A structure used to convert locations to/from coordinate spaces in the hierarchy of the associated SwiftUI view.

let coordinator: Representable.Coordinator

The custom object that you use to communicate state changes from your gesture recognizer to other parts of your SwiftUI interface.

## See Also

### Integrate gesture recognizer into SwiftUI view hierarchies

protocol UIGestureRecognizerRepresentable

A wrapper for a `UIGestureRecognizer` that you use to integrate that gesture recognizer into your SwiftUI hierarchy.

struct UIGestureRecognizerRepresentableCoordinateSpaceConverter

A proxy structure used to convert locations to/from coordinate spaces in the hierarchy of the SwiftUI view associated with a UIGestureRecognizerRepresentable.

