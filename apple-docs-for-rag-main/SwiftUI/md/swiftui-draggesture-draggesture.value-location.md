

- SwiftUI
- DragGesture
- DragGesture.Value
-  location 

Instance Property

# location

The location of the drag gesture’s current event.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
var location: CGPoint
```

## See Also

### Getting 2D position

var startLocation: CGPoint

The location of the drag gesture’s first event.

var predictedEndLocation: CGPoint

A prediction, based on the current drag velocity, of where the final location will be if dragging stopped now.

var translation: CGSize

The total translation from the start of the drag gesture to the current event of the drag gesture.

var predictedEndTranslation: CGSize

A prediction, based on the current drag velocity, of what the final translation will be if dragging stopped now.

