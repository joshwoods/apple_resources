

- UIKit
- UIViewControllerPreviewing
-  previewingGestureRecognizerForFailureRelationship Deprecated

Instance Property

# previewingGestureRecognizerForFailureRelationship

A gesture recognizer suitable for setting up failure requirements for a preview’s (peek’s) gestures.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
var previewingGestureRecognizerForFailureRelationship: UIGestureRecognizer { get }
```

**Required**

## Discussion

Use this gesture recognizer by implementing a delegate object for it that conforms to the UIGestureRecognizerDelegate protocol. The protocol methods let you prevent a preview (peek) press from interfering with an app’s other supported gestures. For example, you could delay a preview’s presentation until after other gestures fail, or you could allow simultaneous recognition of a press and other gestures during a preview’s presentation.

For more information, see the gestureRecognizer(_:shouldBeRequiredToFailBy:) and gestureRecognizer(_:shouldRequireFailureOf:) methods in UIGestureRecognizerDelegate.

## See Also

### Configuring a source view for a 3D Touch previewing view controller

var sourceRect: CGRect

The rectangle, in the source view’s coordinate system, that responds to a 3D Touch by a user and remains visually sharp while surrounding content blurs.

**Required**

Deprecated

