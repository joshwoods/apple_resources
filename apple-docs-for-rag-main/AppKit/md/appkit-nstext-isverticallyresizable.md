

- AppKit
- NSText
-  isVerticallyResizable 

Instance Property

# isVerticallyResizable

A Boolean that controls whether the receiver changes its height to fit the height of its text.

macOS

``` source
@MainActor
var isVerticallyResizable: Bool { get set }
```

## Discussion

If `flag` is true it does; if `flag` is false it doesn’t.

## See Also

### Constraining size

var maxSize: NSSize

The receiver’s maximum size.

var minSize: NSSize

The receiver’s minimum size.

var isHorizontallyResizable: Bool

A Boolean that controls whether the receiver changes its width to fit the width of its text.

func sizeToFit()

Resizes the receiver to fit its text.

