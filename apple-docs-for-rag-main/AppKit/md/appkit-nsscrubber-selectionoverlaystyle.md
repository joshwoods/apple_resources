

- AppKit
- NSScrubber
-  selectionOverlayStyle 

Instance Property

# selectionOverlayStyle

The style overlaid on selected items.

macOS 10.12.2+

``` source
@MainActor
var selectionOverlayStyle: NSScrubberSelectionStyle? { get set }
```

## Discussion

The default value is `nil`, which specifies no overlay decoration.

You can either choose from one of the built-in selection styles (outlineOverlay or roundedBackground), or you can subclass NSScrubberSelectionStyle to create your own custom selection style.

## See Also

### Configuring the selection appearance

var floatsSelectionViews: Bool

A Boolean value that determines the behavior of the item selection decorations as the scrubber’s selection changes.

var selectionBackgroundStyle: NSScrubberSelectionStyle?

The style applied to the background of selected items.

