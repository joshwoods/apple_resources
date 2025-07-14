

- UIKit
- UIPopoverController
-  arrowDirection Deprecated

Instance Property

# arrowDirection

The direction of the popover’s arrow.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var arrowDirection: UIPopoverArrowDirection { get }
```

## Discussion

The default value of this property is unknown. When you present the popover, the value changes to reflect the actual direction of the arrow being used by the popover. When the popover is subsequently dismissed, the value of this property returns to unknown.

## See Also

### Getting the popover attributes

var isPopoverVisible: Bool

A Boolean value indicating whether the popover is currently visible.

Deprecated

