

- UIKit
- UIViewControllerPreviewing
-  sourceRect Deprecated

Instance Property

# sourceRect

The rectangle, in the source view’s coordinate system, that responds to a 3D Touch by a user and remains visually sharp while surrounding content blurs.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
var sourceRect: CGRect { get set }
```

**Required**

## Discussion

Use this property if you want to specify a preview indication area that is different than the bounds of the view in the sourceView property. Set this property’s value in your object’s previewingContext(_:viewControllerForLocation:) method.

The default value of this property corresponds to the bounds of the view in the sourceView property.

For example, if your source view is a table view, you can set the `sourceRect` property to the frame of the row under the user’s touch. The row then remains visually sharp when a user presses it, while surrounding content blurs, thereby indicating to the user that it is the row being touched that has a preview available.

You can change the value of this property at runtime.

## See Also

### Related Documentation

var sourceView: UIView

A source view, in a previewing view controller’s view hierarchy, responds to a 3D Touch by the user.

**Required**

Deprecated

### Configuring a source view for a 3D Touch previewing view controller

var previewingGestureRecognizerForFailureRelationship: UIGestureRecognizer

A gesture recognizer suitable for setting up failure requirements for a preview’s (peek’s) gestures.

**Required**

Deprecated

