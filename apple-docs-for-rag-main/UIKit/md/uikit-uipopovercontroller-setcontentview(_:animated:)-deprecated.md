

- UIKit
- UIPopoverController
-  setContentView(\_:animated:) Deprecated

Instance Method

# setContentView(\_:animated:)

Sets the view controller responsible for the content portion of the popover.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func setContentView(
    _ viewController: UIViewController,
    animated: Bool
)
```

## Parameters 

`viewController`  

The new view controller whose content should be displayed by the popover.

`animated`  

Specify true if the change of view controllers should be animated or false if the change should occur immediately.

## See Also

### Configuring the popover content

var contentViewController: UIViewController

The view controller responsible for the content portion of the popover.

Deprecated

var contentSize: CGSize

The size of the popover’s content view.

Deprecated

func setContentSize(CGSize, animated: Bool)

Changes the size of the popover’s content view.

Deprecated

var passthroughViews: [UIView]?

An array of views that the user can interact with while the popover is visible.

Deprecated

