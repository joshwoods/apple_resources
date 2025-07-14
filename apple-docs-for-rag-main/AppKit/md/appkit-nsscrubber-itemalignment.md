

- AppKit
- NSScrubber
-  itemAlignment 

Instance Property

# itemAlignment

A setting that specifies the snapping behavior of items in the scrubber.

macOS 10.12.2+

``` source
@MainActor
var itemAlignment: NSScrubber.Alignment { get set }
```

## Discussion

Set the value to something other than NSScrubber.Alignment.none to ensure that an item is aligned with the specified position when the scrubber comes to rest.

The default value is NSScrubber.Alignment.none.

## See Also

### Changing the layout

var scrubberLayout: NSScrubberLayout

An object used to describe the layout of items within the scrubber.

var mode: NSScrubber.Mode

A setting that determines whether interaction with the scrubber is fixed or free.

enum Mode

The scrolling behavior for a scrubber.

enum Alignment

The specified preferred alignment of items within the scrubber, when they come to rest following a user’s scrolling or paging interaction.

var isContinuous: Bool

A Boolean value that, together with the mode property, determines scrubber interaction style.

