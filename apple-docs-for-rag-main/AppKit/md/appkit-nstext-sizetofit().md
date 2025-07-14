

- AppKit
- NSText
-  sizeToFit() 

Instance Method

# sizeToFit()

Resizes the receiver to fit its text.

macOS

``` source
@MainActor
func sizeToFit()
```

## Discussion

The text view will not be sized any smaller than its minimum size, however.

## See Also

### Constraining size

var maxSize: NSSize

The receiver’s maximum size.

var minSize: NSSize

The receiver’s minimum size.

var isVerticallyResizable: Bool

A Boolean that controls whether the receiver changes its height to fit the height of its text.

var isHorizontallyResizable: Bool

A Boolean that controls whether the receiver changes its width to fit the width of its text.

