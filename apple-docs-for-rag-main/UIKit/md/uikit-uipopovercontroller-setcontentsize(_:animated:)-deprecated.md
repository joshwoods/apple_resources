

- UIKit
- UIPopoverController
-  setContentSize(\_:animated:) Deprecated

Instance Method

# setContentSize(\_:animated:)

Changes the size of the popover’s content view.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func setContentSize(
    _ size: CGSize,
    animated: Bool
)
```

## Parameters 

`size`  

The new size to apply to the content view.

`animated`  

Specify true if you want the change in size to be animated or false if you want the change to appear immediately.

## Discussion

When changing the size of the popover’s content, the width value you specify must be at least 320 points and no more than 600 points. There are no restrictions on the height value. However, both the width and height values you specify may be adjusted to ensure the popup fits on screen and is not covered by the keyboard.

## See Also

### Configuring the popover content

var contentViewController: UIViewController

The view controller responsible for the content portion of the popover.

Deprecated

func setContentView(UIViewController, animated: Bool)

Sets the view controller responsible for the content portion of the popover.

Deprecated

var contentSize: CGSize

The size of the popover’s content view.

Deprecated

var passthroughViews: [UIView]?

An array of views that the user can interact with while the popover is visible.

Deprecated

