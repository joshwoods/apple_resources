

- AppKit
- NSText
-  isHorizontallyResizable 

Instance Property

# isHorizontallyResizable

A Boolean that controls whether the receiver changes its width to fit the width of its text.

macOS

``` source
@MainActor
var isHorizontallyResizable: Bool { get set }
```

## Discussion

If `flag` is true it does; if `flag` is false it doesn’t

## See Also

### Constraining size

var maxSize: NSSize

The receiver’s maximum size.

var minSize: NSSize

The receiver’s minimum size.

var isVerticallyResizable: Bool

A Boolean that controls whether the receiver changes its height to fit the height of its text.

func sizeToFit()

Resizes the receiver to fit its text.

