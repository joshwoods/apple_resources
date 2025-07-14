

- AppKit
- NSPopoverTouchBarItem
-  collapsedRepresentationLabel 

Instance Property

# collapsedRepresentationLabel

The localized string displayed by the button for the default collapsed representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var collapsedRepresentationLabel: String { get set }
```

## Discussion

If the collapsedRepresentation button has been replaced by a different view, this property may not have any effect.

## See Also

### Configuring the collapsed popover

var collapsedRepresentation: NSView

The view displayed when this item is displayed in its parent bar.

var collapsedRepresentationImage: UIImage?

The image displayed by the button for the default collapsed representation.

