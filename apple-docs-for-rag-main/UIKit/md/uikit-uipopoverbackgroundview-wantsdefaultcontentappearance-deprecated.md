

- UIKit
- UIPopoverBackgroundView
-  wantsDefaultContentAppearance Deprecated

Type Property

# wantsDefaultContentAppearance

Determines whether the default content appearance should be used for the popover.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
class var wantsDefaultContentAppearance: Bool { get }
```

## Discussion

This method may be overridden to prevent the drawing of the content inset and drop shadow inside the popover. The default implementation of this method returns true, which means that the content inset and drop shadow will be drawn. Overriding this method simply means implementing it to return false, which would mean that the content inset and drop shadow will not be drawn.

