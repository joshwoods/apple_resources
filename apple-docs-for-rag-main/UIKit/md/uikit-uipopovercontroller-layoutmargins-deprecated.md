

- UIKit
- UIPopoverController
-  layoutMargins Deprecated

Instance Property

# layoutMargins

The margins that define the portion of the screen in which it is permissible to display the popover.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var layoutMargins: UIEdgeInsets { get set }
```

## Discussion

The edge inset values are measured in points from the edges of the screen, relative to the current device orientation. Thus, the top-edge inset always reflects the top edge of the device from the user’s perspective, which changes depending on whether the user is holding the device in a portrait or landscape orientation. Remember that the device orientation is not always the same as the interface orientation—that is, the orientation of your window and views. Window orientations are typically fixed and view orientations are controlled by the owning view controller. In addition, if the rotation lock option is engaged, the interface does not change orientation at all, even when the device orientation changes.

The default edge insets are 10 points along each edge. The popover controller automatically subtracts the status bar from the viable area when determining where to display the popover, so you do not need to factor the status bar height into your insets.

## See Also

### Customizing the popover appearance

var backgroundViewClass: AnyClass?

The class to use for displaying the popover background content.

Deprecated

var backgroundColor: UIColor?

The color of the popover’s backdrop view.

Deprecated

