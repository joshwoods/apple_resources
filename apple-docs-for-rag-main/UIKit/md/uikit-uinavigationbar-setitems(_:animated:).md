

- UIKit
- UINavigationBar
-  setItems(\_:animated:) 

Instance Method

# setItems(\_:animated:)

Replaces the navigation items currently managed by the navigation bar with the specified items.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setItems(
    _ items: [UINavigationItem]?,
    animated: Bool
)
```

## Parameters 

`items`  

The UINavigationItem objects to place in the stack. The front-to-back order of the items in this array represents the new bottom-to-top order of the items in the navigation stack. Thus, the last item added to the array becomes the top item of the navigation stack.

`animated`  

If true, animate the pushing or popping of the top stack item. If false, replace the stack items without any animations.

## Discussion

You can use this method to update or replace the navigation items in the stack without pushing or popping each item explicitly. In addition, this method lets you update the stack without animating the changes, which might be appropriate at launch time when you want to restore the state of the navigation stack to some previous state.

If animations are enabled, this method decides which type of transition to perform based on whether the last item in the items array is already on the current navigation stack. If the item is currently on the stack, but is not the topmost item, this method uses a pop transition; if it is the topmost item, no transition is performed. If the item is not on the stack, this method uses a push transition. Only one transition is performed, but when that transition finishes, the entire contents of the stack are replaced with the new items. For example, if items A, B, and C are on the stack and you set items D, A, and B, this method uses a pop transition and the resulting stack contains the items D, A, and B.

## See Also

### Pushing and popping items

func pushItem(UINavigationItem, animated: Bool)

Pushes the given navigation item onto the navigation bar’s stack and updates the UI.

func popItem(animated: Bool) -> UINavigationItem?

Pops the top item from the navigation bar’s stack and updates the UI.

var items: [UINavigationItem]?

An array of navigation items managed by the navigation bar.

var topItem: UINavigationItem?

The navigation item at the top of the navigation bar’s stack.

var backItem: UINavigationItem?

The navigation item that is immediately below the topmost item on a navigation bar’s stack.

