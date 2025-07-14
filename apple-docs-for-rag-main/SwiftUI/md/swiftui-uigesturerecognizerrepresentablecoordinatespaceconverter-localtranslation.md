

- SwiftUI
- UIGestureRecognizerRepresentableCoordinateSpaceConverter
-  localTranslation 

Instance Property

# localTranslation

The represented gesture recognizer’s current translation in the coordinate space of the SwiftUI view it’s attached to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
var localTranslation: CGPoint? { get }
```

## Discussion

If the gesture recognizer does not implement a `translationInView:` method, returns nil.

