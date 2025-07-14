

- UIKit
- UIMenuController
-  setMenuVisible(\_:animated:) Deprecated

Instance Method

# setMenuVisible(\_:animated:)

Shows or hides the editing menu, optionally animating the action.

iOS 3.0–13.0DeprecatediPadOS 3.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func setMenuVisible(
    _ menuVisible: Bool,
    animated: Bool
)
```

## Parameters 

`menuVisible`  

true if the menu should be shown, false if it should be hidden.

`animated`  

true if the showing or hiding of the menu should be animated, otherwise false.

## Discussion

Before showing the menu, be sure to position it relative to the selection. See setTargetRect(_:in:) for details. If you do not set the target rect before displaying the menu, it appears at screen coordinates (0.0, 0.0).

## See Also

### Showing and hiding the menu

func showMenu(from: UIView, rect: CGRect)Deprecated

func hideMenu(from: UIView)Deprecated

func hideMenu()Deprecated

var isMenuVisible: Bool

The visibility of the editing menu.

Deprecated

