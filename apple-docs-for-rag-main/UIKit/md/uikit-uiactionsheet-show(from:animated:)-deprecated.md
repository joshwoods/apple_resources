

- UIKit
- UIActionSheet
-  show(from:animated:) Deprecated

Instance Method

# show(from:animated:)

Displays an action sheet that originates from the specified bar button item.

iOS 3.2–8.3DeprecatediPadOS 3.2–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func show(
    from item: UIBarButtonItem,
    animated: Bool
)
```

## Parameters 

`item`  

The bar button item from which the action sheet originates.

`animated`  

Specify true to animate the presentation of the action sheet or false to present it immediately without any animation effects.

## Discussion

On iPad, this method presents the action sheet in a popover and adds the toolbar that owns the button to the popover’s list of passthrough views. Thus, taps in the toolbar result in the action methods of the corresponding toolbar items being called. If you want the popover to be dismissed when a different toolbar item is tapped, you must implement that behavior in your action handler methods.

## See Also

### Presenting the action sheet

func show(from: UITabBar)

Displays an action sheet that originates from the specified tab bar.

Deprecated

func show(from: UIToolbar)

Displays an action sheet that originates from the specified toolbar.

Deprecated

func show(in: UIView)

Displays an action sheet that originates from the specified view.

Deprecated

func show(from: CGRect, in: UIView, animated: Bool)

Displays an action sheet that originates from the specified view.

Deprecated

