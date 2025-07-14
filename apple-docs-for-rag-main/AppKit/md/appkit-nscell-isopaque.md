

- AppKit
- NSCell
-  isOpaque 

Instance Property

# isOpaque

A Boolean value indicating whether the cell is completely opaque.

macOS

``` source
@MainActor
var isOpaque: Bool { get }
```

## Discussion

The value of this property is true if the cell is completely opaque or false if it contains some transparency.

## See Also

### Managing Display Attributes

var isBezeled: Bool

A Boolean value indicating whether the cell has a bezeled border.

var isBordered: Bool

A Boolean value indicating whether the cell draws itself outlined with a plain border.

var controlTint: NSControlTint

The cell’s control tint.

Deprecated

var backgroundStyle: NSView.BackgroundStyle

The cell’s background style.

var interiorBackgroundStyle: NSView.BackgroundStyle

The cell’s interior background style.

enum BackgroundStyle

Background styles to apply to a view’s cell.

