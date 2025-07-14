

- UIKit
- UINavigationBar
-  backItem 

Instance Property

# backItem

The navigation item that is immediately below the topmost item on a navigation bar’s stack.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var backItem: UINavigationItem? { get }
```

## Discussion

If the leftBarButtonItem property of the topmost navigation item is `nil`, the navigation bar displays a back button whose title is derived from the item in this property.

If there is only one item on the navigation bar’s stack, the value of this property is `nil`.

## See Also

### Pushing and popping items

func pushItem(UINavigationItem, animated: Bool)

Pushes the given navigation item onto the navigation bar’s stack and updates the UI.

func popItem(animated: Bool) -> UINavigationItem?

Pops the top item from the navigation bar’s stack and updates the UI.

func setItems([UINavigationItem]?, animated: Bool)

Replaces the navigation items currently managed by the navigation bar with the specified items.

var items: [UINavigationItem]?

An array of navigation items managed by the navigation bar.

var topItem: UINavigationItem?

The navigation item at the top of the navigation bar’s stack.

