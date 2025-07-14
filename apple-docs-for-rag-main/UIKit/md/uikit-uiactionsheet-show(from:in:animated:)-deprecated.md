

- UIKit
- UIActionSheet
-  show(from:in:animated:) Deprecated

Instance Method

# show(from:in:animated:)

Displays an action sheet that originates from the specified view.

iOS 3.2–8.3DeprecatediPadOS 3.2–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func show(
    from rect: CGRect,
    in view: UIView,
    animated: Bool
)
```

## Parameters 

`rect`  

The portion of `view` from which to originate the action sheet.

`view`  

The view from which to originate the action sheet.

`animated`  

Specify true to animate the presentation of the action sheet or false to present it immediately without any animation effects.

## Discussion

On iPad, this method displays the action sheet in a popover whose arrow points to the specified rectangle of the view. The popover does not overlap the specified rectangle.

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

func show(from: UIBarButtonItem, animated: Bool)

Displays an action sheet that originates from the specified bar button item.

Deprecated

