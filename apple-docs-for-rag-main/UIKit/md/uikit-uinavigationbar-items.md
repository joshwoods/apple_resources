

- UIKit
- UINavigationBar
-  items 

Instance Property

# items

An array of navigation items managed by the navigation bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var items: [UINavigationItem]? { get set }
```

## Discussion

The bottom item is at index `0`, the back item is at index `n-2`, and the top item is at index `n-1`, where `n` is the number of items in the array.

## See Also

### Pushing and popping items

func pushItem(UINavigationItem, animated: Bool)

Pushes the given navigation item onto the navigation bar’s stack and updates the UI.

func popItem(animated: Bool) -> UINavigationItem?

Pops the top item from the navigation bar’s stack and updates the UI.

func setItems([UINavigationItem]?, animated: Bool)

Replaces the navigation items currently managed by the navigation bar with the specified items.

var topItem: UINavigationItem?

The navigation item at the top of the navigation bar’s stack.

var backItem: UINavigationItem?

The navigation item that is immediately below the topmost item on a navigation bar’s stack.

