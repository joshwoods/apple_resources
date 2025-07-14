

- AppKit
- NSPopoverTouchBarItem
-  collapsedRepresentation 

Instance Property

# collapsedRepresentation

The view displayed when this item is displayed in its parent bar.

macOS 10.12.2+

``` source
@MainActor
var collapsedRepresentation: NSView { get set }
```

## Discussion

By default, this is an NSButton whose target is this popover item, whose action is showPopover(_:), and whose image and title are bound to this item’s collapsedRepresentationImage and collapsedRepresentationImage respectively.

## See Also

### Configuring the collapsed popover

var collapsedRepresentationImage: UIImage?

The image displayed by the button for the default collapsed representation.

var collapsedRepresentationLabel: String

The localized string displayed by the button for the default collapsed representation.

