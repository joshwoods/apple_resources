

- UIKit
- UIPopoverController
-  backgroundColor Deprecated

Instance Property

# backgroundColor

The color of the popover’s backdrop view.

iOS 7.0–9.0DeprecatediPadOS 7.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@NSCopying @MainActor
var backgroundColor: UIColor? { get set }
```

## Discussion

Use this property to customize the background color of your popover. Changing the value of this property while the popover is visible triggers an animated changeover to the new color. The default value of this property is `nil`, which corresponds to the default background color.

## See Also

### Customizing the popover appearance

var layoutMargins: UIEdgeInsets

The margins that define the portion of the screen in which it is permissible to display the popover.

Deprecated

var backgroundViewClass: AnyClass?

The class to use for displaying the popover background content.

Deprecated

