

- UIKit
- UIPopoverController
-  backgroundViewClass Deprecated

Instance Property

# backgroundViewClass

The class to use for displaying the popover background content.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var backgroundViewClass: AnyClass? { get set }
```

## Discussion

The default value of this property is `nil`, which indicates that the popover controller should use the default popover appearance. Setting this property to a value other than `nil` causes the popover controller to use the specified class to draw the popover’s background content. The class you specify must be a subclass of UIPopoverBackgroundView.

## See Also

### Customizing the popover appearance

var layoutMargins: UIEdgeInsets

The margins that define the portion of the screen in which it is permissible to display the popover.

Deprecated

var backgroundColor: UIColor?

The color of the popover’s backdrop view.

Deprecated

