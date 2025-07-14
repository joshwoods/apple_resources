

- AppKit
- NSScrubber
-  backgroundView 

Instance Property

# backgroundView

A view that is displayed behind the scrubber content.

macOS 10.12.2+

``` source
@MainActor
var backgroundView: NSView? { get set }
```

## Discussion

The scrubber manages the layout of the background view to match the size of the content area. If this property is non-`nil`, the value of the backgroundColor property is ignored.

The default value is `nil`.

## See Also

### Configuring the scrubber’s appearance

var backgroundColor: NSColor?

The color displayed behind the scrubber content.

var showsAdditionalContentIndicators: Bool

A Boolean value that specifies whether the scrubber should display the existence of additional items beyond the leading and trailing edges.

var showsArrowButtons: Bool

A Boolean value that specifies whether arrow buttons should be displayed at the leading and trailing edges of the scrubber.

