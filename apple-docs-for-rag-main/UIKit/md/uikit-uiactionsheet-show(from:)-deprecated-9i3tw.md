

- UIKit
- UIActionSheet
-  show(from:) Deprecated

Instance Method

# show(from:)

Displays an action sheet that originates from the specified tab bar.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func show(from view: UITabBar)
```

## Parameters 

`view`  

The tab bar from which the action sheet originates.

## Discussion

The appearance of the action sheet is animated.

On iPad, this method centers the action sheet in the middle of the screen. Generally, if you want to present an action sheet relative to a tab bar in an iPad application, you should use the show(from:in:animated:) method instead.

## See Also

### Presenting the action sheet

func show(from: UIToolbar)

Displays an action sheet that originates from the specified toolbar.

Deprecated

func show(in: UIView)

Displays an action sheet that originates from the specified view.

Deprecated

func show(from: UIBarButtonItem, animated: Bool)

Displays an action sheet that originates from the specified bar button item.

Deprecated

func show(from: CGRect, in: UIView, animated: Bool)

Displays an action sheet that originates from the specified view.

Deprecated

