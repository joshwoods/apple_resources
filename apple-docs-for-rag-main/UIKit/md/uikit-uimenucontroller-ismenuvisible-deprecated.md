

- UIKit
- UIMenuController
-  isMenuVisible Deprecated

Instance Property

# isMenuVisible

The visibility of the editing menu.

iOS 3.0–16.0DeprecatediPadOS 3.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var isMenuVisible: Bool { get set }
```

## Discussion

Setting this property displays or hides the menu immediately, without animation. For animating the showing or hiding of the menu, use the setMenuVisible(_:animated:) method. Before showing the menu, be sure to position it relative to the selection.

## See Also

### Showing and hiding the menu

func showMenu(from: UIView, rect: CGRect)Deprecated

func hideMenu(from: UIView)Deprecated

func hideMenu()Deprecated

func setMenuVisible(Bool, animated: Bool)

Shows or hides the editing menu, optionally animating the action.

Deprecated

