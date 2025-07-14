

- AppKit
- NSScrubber
-  selectionBackgroundStyle 

Instance Property

# selectionBackgroundStyle

The style applied to the background of selected items.

macOS 10.12.2+

``` source
@MainActor
var selectionBackgroundStyle: NSScrubberSelectionStyle? { get set }
```

## Discussion

The default value is `nil`, which specifies no background decoration.

You can either choose from one of the built-in selection styles (outlineOverlay or roundedBackground), or you can subclass NSScrubberSelectionStyle to create your own custom selection style.

## See Also

### Configuring the selection appearance

var floatsSelectionViews: Bool

A Boolean value that determines the behavior of the item selection decorations as the scrubber’s selection changes.

var selectionOverlayStyle: NSScrubberSelectionStyle?

The style overlaid on selected items.

