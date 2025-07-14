

- AppKit
- NSCell
-  controlTint Deprecated

Instance Property

# controlTint

The cell’s control tint.

macOS 10.0–11.0Deprecated

``` source
@MainActor
var controlTint: NSControlTint { get set }
```

Deprecated

The controlTint property is not respected on 10.14 and later. For custom cells, use +\[NSColor controlAccentColor\] to respect the user's preferred accent color when drawing.

## Discussion

The default value of this property is NSControlTint.defaultControlTint.

## See Also

### Managing Display Attributes

var isBezeled: Bool

A Boolean value indicating whether the cell has a bezeled border.

var isBordered: Bool

A Boolean value indicating whether the cell draws itself outlined with a plain border.

var isOpaque: Bool

A Boolean value indicating whether the cell is completely opaque.

var backgroundStyle: NSView.BackgroundStyle

The cell’s background style.

var interiorBackgroundStyle: NSView.BackgroundStyle

The cell’s interior background style.

enum BackgroundStyle

Background styles to apply to a view’s cell.

