

- AppKit
- NSScrubber
-  showsAdditionalContentIndicators 

Instance Property

# showsAdditionalContentIndicators

A Boolean value that specifies whether the scrubber should display the existence of additional items beyond the leading and trailing edges.

macOS 10.12.2+

``` source
@MainActor
var showsAdditionalContentIndicators: Bool { get set }
```

## Discussion

When true, the scrubber uses a fade effect to indicate that there is additional content the user can scroll to. The default value is false.

## See Also

### Configuring the scrubber’s appearance

var backgroundColor: NSColor?

The color displayed behind the scrubber content.

var backgroundView: NSView?

A view that is displayed behind the scrubber content.

var showsArrowButtons: Bool

A Boolean value that specifies whether arrow buttons should be displayed at the leading and trailing edges of the scrubber.

