

- UIKit
- UIMenuController
-  arrowDirection Deprecated

Instance Property

# arrowDirection

The direction the arrow of the editing menu is pointing.

iOS 3.2–16.0DeprecatediPadOS 3.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var arrowDirection: UIMenuController.ArrowDirection { get set }
```

## Discussion

You can set the direction editing-menu arrow points by assigning a UIMenuController.ArrowDirection enum constant to this property. The default behavior (UIMenuController.ArrowDirection.default) is to point up or down at the object of focus based on its location on the screen.

## See Also

### Positioning the menu

var menuFrame: CGRect

Returns the frame of the editing menu.

Deprecated

enum ArrowDirection

The direction the arrow of the editing menu is pointing.

Deprecated

func setTargetRect(CGRect, in: UIView)

Sets the area in a view above or below which the editing menu is positioned.

Deprecated

