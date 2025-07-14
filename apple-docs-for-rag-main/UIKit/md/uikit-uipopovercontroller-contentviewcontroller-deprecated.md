

- UIKit
- UIPopoverController
-  contentViewController Deprecated

Instance Property

# contentViewController

The view controller responsible for the content portion of the popover.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var contentViewController: UIViewController { get set }
```

## Discussion

This property is initially set to the view controller passed to the init(contentViewController:) method. You can change the value of this property later to reflect a new set of content. Changing the value of this property swaps the new view controller in for the old one immediately and does not trigger an animation. If you want to animate the change, use the setContentView(_:animated:) method instead.

## See Also

### Configuring the popover content

func setContentView(UIViewController, animated: Bool)

Sets the view controller responsible for the content portion of the popover.

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

