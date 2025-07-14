

- AppKit
- NSPopoverTouchBarItem
-  collapsedRepresentationImage 

Instance Property

# collapsedRepresentationImage

The image displayed by the button for the default collapsed representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

**macOS**

``` source
@MainActor
var collapsedRepresentationImage: NSImage? { get set }
```

**Mac Catalyst**

``` source
@MainActor
var collapsedRepresentationImage: UIImage? { get set }
```

## Discussion

If the collapsedRepresentation button has been replaced by a different view, this property may not have any effect.

## See Also

### Configuring the collapsed popover

var collapsedRepresentation: NSView

The view displayed when this item is displayed in its parent bar.

var collapsedRepresentationLabel: String

The localized string displayed by the button for the default collapsed representation.

