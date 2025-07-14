

- AppKit
- NSCell
-  interiorBackgroundStyle 

Instance Property

# interiorBackgroundStyle

The cell’s interior background style.

macOS 10.5+

``` source
@MainActor
var interiorBackgroundStyle: NSView.BackgroundStyle { get }
```

## Discussion

The interior background style describes the surface drawn onto in the drawInterior(withFrame:in:) method. This is often the same as the backgroundStyle, but a button that draws a bezel would use a different value for this property.

In a custom button with a custom bezel you can override this property and return a different value to describe that surface. A cell that has custom interior drawing might use the value of this property to pick an image that looks good on the cell.

## See Also

### Managing Display Attributes

var isBezeled: Bool

A Boolean value indicating whether the cell has a bezeled border.

var isBordered: Bool

A Boolean value indicating whether the cell draws itself outlined with a plain border.

var isOpaque: Bool

A Boolean value indicating whether the cell is completely opaque.

var controlTint: NSControlTint

The cell’s control tint.

Deprecated

var backgroundStyle: NSView.BackgroundStyle

The cell’s background style.

enum BackgroundStyle

Background styles to apply to a view’s cell.

