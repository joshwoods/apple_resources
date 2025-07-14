

- UIKit
- UIPopoverController
-  contentSize Deprecated

Instance Property

# contentSize

The size of the popover’s content view.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var contentSize: CGSize { get set }
```

## Discussion

This property represents the size of the content view that is managed by the view controller in the contentViewController property. The initial value of this property is set to value in the view controller’s contentSizeForViewInPopover property. Changing the value of this property overrides the default value of the current view controller. The overridden value persists until you assign a new content view controller to the receiver. Thus, if you want to keep your overridden value, you must reassign it after changing the content view controller.

When changing the value of this property, the width value you specify must be at least 320 points and no more than 600 points. There are no restrictions on the height value. However, both the width and height values you specify may be adjusted to ensure the popup fits on screen and is not covered by the keyboard. If you change the value of this property while the popover is visible, the size change is animated.

## See Also

### Configuring the popover content

var contentViewController: UIViewController

The view controller responsible for the content portion of the popover.

Deprecated

func setContentView(UIViewController, animated: Bool)

Sets the view controller responsible for the content portion of the popover.

Deprecated

func setContentSize(CGSize, animated: Bool)

Changes the size of the popover’s content view.

Deprecated

var passthroughViews: [UIView]?

An array of views that the user can interact with while the popover is visible.

Deprecated

