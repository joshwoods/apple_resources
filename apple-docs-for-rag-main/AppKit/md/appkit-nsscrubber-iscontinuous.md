

- AppKit
- NSScrubber
-  isContinuous 

Instance Property

# isContinuous

A Boolean value that, together with the mode property, determines scrubber interaction style.

macOS 10.12.2+

``` source
@MainActor
var isContinuous: Bool { get set }
```

## Discussion

For details on how to choose the right isContinuous value for your app, see Choose a scrubber touch-interaction model.

## See Also

### Changing the layout

var scrubberLayout: NSScrubberLayout

An object used to describe the layout of items within the scrubber.

var mode: NSScrubber.Mode

A setting that determines whether interaction with the scrubber is fixed or free.

enum Mode

The scrolling behavior for a scrubber.

var itemAlignment: NSScrubber.Alignment

A setting that specifies the snapping behavior of items in the scrubber.

enum Alignment

The specified preferred alignment of items within the scrubber, when they come to rest following a user’s scrolling or paging interaction.

