

- UIKit
- UINavigationBar
-  popItem(animated:) 

Instance Method

# popItem(animated:)

Pops the top item from the navigation bar’s stack and updates the UI.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func popItem(animated: Bool) -> UINavigationItem?
```

## Parameters 

`animated`  

true if the navigation bar should be animated; otherwise, false.

## Return Value

The top item that was popped.

## Discussion

Popping a navigation item removes the top item from the stack and replaces it with the back item. The back item’s title is centered on the navigation bar and its other properties are displayed.

## See Also

### Pushing and popping items

func pushItem(UINavigationItem, animated: Bool)

Pushes the given navigation item onto the navigation bar’s stack and updates the UI.

func setItems([UINavigationItem]?, animated: Bool)

Replaces the navigation items currently managed by the navigation bar with the specified items.

var items: [UINavigationItem]?

An array of navigation items managed by the navigation bar.

var topItem: UINavigationItem?

The navigation item at the top of the navigation bar’s stack.

var backItem: UINavigationItem?

The navigation item that is immediately below the topmost item on a navigation bar’s stack.

