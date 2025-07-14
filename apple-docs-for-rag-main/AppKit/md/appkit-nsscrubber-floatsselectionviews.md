

- AppKit
- NSScrubber
-  floatsSelectionViews 

Instance Property

# floatsSelectionViews

A Boolean value that determines the behavior of the item selection decorations as the scrubber’s selection changes.

macOS 10.12.2+

``` source
@MainActor
var floatsSelectionViews: Bool { get set }
```

## Discussion

When scrubber items are selected, they are decorated with background and overlay views, as determined by the selectionBackgroundStyle and selectionOverlayStyle properties.

As the selection changes, the behavior of these selection decoration views is determined by the floatsSelectionViews property, as follows:

- true The overlay and background views float smoothly between the previously selected item and the newly selected item.

- false The overlay and background views cross-fade from the previously selected item to the newly selected item.

The default value is false.

## See Also

### Configuring the selection appearance

var selectionOverlayStyle: NSScrubberSelectionStyle?

The style overlaid on selected items.

var selectionBackgroundStyle: NSScrubberSelectionStyle?

The style applied to the background of selected items.

