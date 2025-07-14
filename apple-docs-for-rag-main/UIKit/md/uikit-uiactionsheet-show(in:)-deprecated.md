

- UIKit
- UIActionSheet
-  show(in:) Deprecated

Instance Method

# show(in:)

Displays an action sheet that originates from the specified view.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func show(in view: UIView)
```

## Parameters 

`view`  

The view from which the action sheet originates.

## Discussion

The appearance of the action sheet is animated.

On iPad, this method centers the action sheet in the middle of the screen. Generally, if you want to present an action sheet in an iPad application, you should use the show(from:in:animated:) method to display the action sheet instead.

## See Also

### Presenting the action sheet

func show(from: UITabBar)

Displays an action sheet that originates from the specified tab bar.

Deprecated

func show(from: UIToolbar)

Displays an action sheet that originates from the specified toolbar.

Deprecated

func show(from: UIBarButtonItem, animated: Bool)

Displays an action sheet that originates from the specified bar button item.

Deprecated

func show(from: CGRect, in: UIView, animated: Bool)

Displays an action sheet that originates from the specified view.

Deprecated

