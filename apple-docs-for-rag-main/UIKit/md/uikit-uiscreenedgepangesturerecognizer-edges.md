

- UIKit
- UIScreenEdgePanGestureRecognizer
-  edges 

Instance Property

# edges

The acceptable starting edges for the gesture.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+

``` source
@MainActor
var edges: UIRectEdge { get set }
```

## Mentioned in 

Handling pan gestures

## Discussion

The edges you specify are always relative to the app’s current interface orientation. This behavior ensures that the gestures always occur from the same place in your user interface, regardless of the device’s current orientation.

## See Also

### Specifying the starting edges

struct UIRectEdge

Constants that specify the edges of a rectangle.

