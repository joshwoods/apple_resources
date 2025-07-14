

- UIKit
- UITabBar
-  setItems(\_:animated:) 

Instance Method

# setItems(\_:animated:)

Sets the items on the tab bar, optionally animating any changes into position.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setItems(
    _ items: [UITabBarItem]?,
    animated: Bool
)
```

## Parameters 

`items`  

The array of UITabBarItem objects to display.

`animated`  

A Boolean indicating whether changes should be animated. Specify true to animate changes or false to display the new items without animations. When animations are enabled, the tab bar fades out removed items and fades in new items, adjusting the spacing between items as needed.

## Discussion

Use this method to make changes to the currently visible items at runtime. Calling this method on a tab bar that is managed by a UITabBarController object raises an exception. When the tab bar is owned by a tab bar controller, use the tab bar controller’s methods to make changes to items.

## See Also

### Configuring tab bar items

var items: [UITabBarItem]?

The items displayed by the tab bar.

var selectedItem: UITabBarItem?

The currently selected item on the tab bar.

