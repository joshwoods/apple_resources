

- AppKit
- NSScrubber
-  mode 

Instance Property

# mode

A setting that determines whether interaction with the scrubber is fixed or free.

macOS 10.12.2+

``` source
@MainActor
var mode: NSScrubber.Mode { get set }
```

## Discussion

When set to NSScrubber.Mode.fixed, the scrubber’s content doesn’t scroll as the user pans. Instead, the element under the user’s finger is highlighted. The highlighted item becomes selected when the user completes the pan gesture. The default value is NSScrubber.Mode.fixed.

When mode is set to NSScrubber.Mode.free, panning over the scrubber scrolls the scrubber’s content. A user selects items by tapping on them.

## See Also

### Changing the layout

var scrubberLayout: NSScrubberLayout

An object used to describe the layout of items within the scrubber.

enum Mode

The scrolling behavior for a scrubber.

var itemAlignment: NSScrubber.Alignment

A setting that specifies the snapping behavior of items in the scrubber.

enum Alignment

The specified preferred alignment of items within the scrubber, when they come to rest following a user’s scrolling or paging interaction.

var isContinuous: Bool

A Boolean value that, together with the mode property, determines scrubber interaction style.

