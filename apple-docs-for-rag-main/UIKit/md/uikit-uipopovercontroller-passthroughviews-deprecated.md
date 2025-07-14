

- UIKit
- UIPopoverController
-  passthroughViews Deprecated

Instance Property

# passthroughViews

An array of views that the user can interact with while the popover is visible.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var passthroughViews: [UIView]? { get set }
```

## Discussion

When a popover is active, interactions with other views are normally disabled until the popover is dismissed. Assigning an array of views to this property allows taps outside of the popover to be handled by the corresponding views.

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

func setContentSize(CGSize, animated: Bool)

Changes the size of the popover’s content view.

Deprecated

