

- AppKit
- NSScrubber
-  backgroundColor 

Instance Property

# backgroundColor

The color displayed behind the scrubber content.

macOS 10.12.2+

``` source
@NSCopying @MainActor
var backgroundColor: NSColor? { get set }
```

## Discussion

The value of this property is ignored if the value of the backgroundView property is non-`nil`. The default value is `nil`.

## See Also

### Configuring the scrubber’s appearance

var backgroundView: NSView?

A view that is displayed behind the scrubber content.

var showsAdditionalContentIndicators: Bool

A Boolean value that specifies whether the scrubber should display the existence of additional items beyond the leading and trailing edges.

var showsArrowButtons: Bool

A Boolean value that specifies whether arrow buttons should be displayed at the leading and trailing edges of the scrubber.

