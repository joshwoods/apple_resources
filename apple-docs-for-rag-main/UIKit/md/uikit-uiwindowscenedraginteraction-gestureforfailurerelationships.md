

- UIKit
- UIWindowSceneDragInteraction
-  gestureForFailureRelationships 

Instance Property

# gestureForFailureRelationships

The gesture that the drag interaction adds to the view hierarchy.

iOS 17.0+iPadOS 17.0+visionOS 1.0+

``` source
@MainActor
var gestureForFailureRelationships: UIGestureRecognizer { get }
```

## Discussion

If your app provides other gestures in the same view hierarchy, you may want to set up failure requirements between your app’s gestures and the drag interaction’s gesture. To do this, use the require(toFail:) method to relate your gestures to this gesture. For example:

- Swift
- Objective-C

```
windowDragInteraction.gestureForFailureRelationships.require(toFail: swipeGesture)
```

```
[windowDragInteraction.gestureForFailureRelationships requireGestureRecognizerToFail:self.swipeGesture];
```

