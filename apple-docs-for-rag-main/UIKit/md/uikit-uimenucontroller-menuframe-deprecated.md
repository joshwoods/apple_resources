

- UIKit
- UIMenuController
-  menuFrame Deprecated

Instance Property

# menuFrame

Returns the frame of the editing menu.

iOS 3.0–16.0DeprecatediPadOS 3.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var menuFrame: CGRect { get }
```

## Discussion

The property value is the bounding rectangle of the menu in screen coordinates. The property has a value of CGRectZero if the menu is not visible. You can use this property to adjust any user-interface objects away from the menu after displaying the menu.

## See Also

### Positioning the menu

var arrowDirection: UIMenuController.ArrowDirection

The direction the arrow of the editing menu is pointing.

Deprecated

enum ArrowDirection

The direction the arrow of the editing menu is pointing.

Deprecated

func setTargetRect(CGRect, in: UIView)

Sets the area in a view above or below which the editing menu is positioned.

Deprecated

