

- UIKit
- UIMenuController
-  setTargetRect(\_:in:) Deprecated

Instance Method

# setTargetRect(\_:in:)

Sets the area in a view above or below which the editing menu is positioned.

iOS 3.0–13.0DeprecatediPadOS 3.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func setTargetRect(
    _ targetRect: CGRect,
    in targetView: UIView
)
```

Deprecated

Use showMenuFromView:rect: instead.

## Parameters 

`targetRect`  

A rectangle that defines the area that is to be the target of the menu commands.

`targetView`  

The view in which `targetRect` appears.

## Discussion

This target rectangle (`targetRect`) is usually the bounding rectangle of a selection. `UIMenuController` positions the editing menu above this rectangle; if there is not enough space for the menu there, it positions it below the rectangle. The menu’s pointer is placed at the center of the top or bottom of the target rectangle as appropriate. Note that if you make the width or height of the target rectangle zero, `UIMenuController` treats the target area as a line or point for positioning (for example, an insertion caret or a single point).

Once it is set, the target rectangle does not track the view; if the view moves (such as would happen in a scroll view), you must update the target rectangle accordingly.

## See Also

### Positioning the menu

var menuFrame: CGRect

Returns the frame of the editing menu.

Deprecated

var arrowDirection: UIMenuController.ArrowDirection

The direction the arrow of the editing menu is pointing.

Deprecated

enum ArrowDirection

The direction the arrow of the editing menu is pointing.

Deprecated

