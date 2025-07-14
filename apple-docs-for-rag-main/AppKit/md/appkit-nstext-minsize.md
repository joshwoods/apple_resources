

- AppKit
- NSText
-  minSize 

Instance Property

# minSize

The receiver’s minimum size.

macOS

``` source
@MainActor
var minSize: NSSize { get set }
```

## See Also

### Constraining size

var maxSize: NSSize

The receiver’s maximum size.

var isVerticallyResizable: Bool

A Boolean that controls whether the receiver changes its height to fit the height of its text.

var isHorizontallyResizable: Bool

A Boolean that controls whether the receiver changes its width to fit the width of its text.

func sizeToFit()

Resizes the receiver to fit its text.

