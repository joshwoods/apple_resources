

- AppKit
- NSText
-  drawsBackground 

Instance Property

# drawsBackground

A Boolean that controls whether the receiver draws its background.

macOS

``` source
@MainActor
var drawsBackground: Bool { get set }
```

## Discussion

If `flag` is true, the receiver fills its background with the background color, if `flag` is false, it doesn’t.

## See Also

### Setting graphics attributes

var backgroundColor: NSColor?

The receiver’s background color to a given color.

