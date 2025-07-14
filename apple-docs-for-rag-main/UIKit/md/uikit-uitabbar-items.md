

- UIKit
- UITabBar
-  items 

Instance Property

# items

The items displayed by the tab bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var items: [UITabBarItem]? { get set }
```

## Discussion

This property contains an array of UITabBarItem objects, each of which corresponds to a tab displayed by the tab bar. The order of the items in this property corresponds to the order of the items onscreen. You can use this property to access the items as needed.

For tab bars you create, you can assign a new set of items to this property to change the displayed items. Changing the items replaces them immediately without animations. You must not modify this property if the tab bar is managed by a UITabBarController object, and doing so raises an exception. When the tab bar is owned by a tab bar controller, use the tab bar controller’s methods to make changes.

The default value of this property is `nil`.

## See Also

### Configuring tab bar items

func setItems([UITabBarItem]?, animated: Bool)

Sets the items on the tab bar, optionally animating any changes into position.

var selectedItem: UITabBarItem?

The currently selected item on the tab bar.

