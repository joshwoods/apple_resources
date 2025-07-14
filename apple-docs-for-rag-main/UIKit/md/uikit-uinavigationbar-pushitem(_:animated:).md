

- UIKit
- UINavigationBar
-  pushItem(\_:animated:) 

Instance Method

# pushItem(\_:animated:)

Pushes the given navigation item onto the navigation bar’s stack and updates the UI.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func pushItem(
    _ item: UINavigationItem,
    animated: Bool
)
```

## Parameters 

`item`  

The navigation item to push on the stack.

`animated`  

true if the navigation bar should be animated; otherwise, false.

## Discussion

Pushing a navigation item displays the item’s title in the center on the navigation bar. The previous top navigation item (if it exists) is displayed as a Back button on the left side of the navigation bar. If the new top item has a left custom view, it is displayed instead of the back button.

## See Also

### Pushing and popping items

func popItem(animated: Bool) -> UINavigationItem?

Pops the top item from the navigation bar’s stack and updates the UI.

func setItems([UINavigationItem]?, animated: Bool)

Replaces the navigation items currently managed by the navigation bar with the specified items.

var items: [UINavigationItem]?

An array of navigation items managed by the navigation bar.

var topItem: UINavigationItem?

The navigation item at the top of the navigation bar’s stack.

var backItem: UINavigationItem?

The navigation item that is immediately below the topmost item on a navigation bar’s stack.

