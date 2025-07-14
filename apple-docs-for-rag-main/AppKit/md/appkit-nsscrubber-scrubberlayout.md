

- AppKit
- NSScrubber
-  scrubberLayout 

Instance Property

# scrubberLayout

An object used to describe the layout of items within the scrubber.

macOS 10.12.2+

``` source
@MainActor
var scrubberLayout: NSScrubberLayout { get set }
```

## See Also

### Changing the layout

var mode: NSScrubber.Mode

A setting that determines whether interaction with the scrubber is fixed or free.

enum Mode

The scrolling behavior for a scrubber.

var itemAlignment: NSScrubber.Alignment

A setting that specifies the snapping behavior of items in the scrubber.

enum Alignment

The specified preferred alignment of items within the scrubber, when they come to rest following a user’s scrolling or paging interaction.

var isContinuous: Bool

A Boolean value that, together with the mode property, determines scrubber interaction style.

