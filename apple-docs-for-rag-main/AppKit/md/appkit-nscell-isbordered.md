

- AppKit
- NSCell
-  isBordered 

Instance Property

# isBordered

A Boolean value indicating whether the cell draws itself outlined with a plain border.

macOS

``` source
@MainActor
var isBordered: Bool { get set }
```

## Discussion

The value of this property is true if the cell has a plain border or false if it does not. This property is mutually exclusive with the isBezeled property—that is, a cell’s border can be plain or bezeled but not both. Changing the value of this property automatically removes any bezel that has been set, regardless of the value you assign to the property.

## See Also

### Managing Display Attributes

var isBezeled: Bool

A Boolean value indicating whether the cell has a bezeled border.

var isOpaque: Bool

A Boolean value indicating whether the cell is completely opaque.

var controlTint: NSControlTint

The cell’s control tint.

Deprecated

var backgroundStyle: NSView.BackgroundStyle

The cell’s background style.

var interiorBackgroundStyle: NSView.BackgroundStyle

The cell’s interior background style.

enum BackgroundStyle

Background styles to apply to a view’s cell.

