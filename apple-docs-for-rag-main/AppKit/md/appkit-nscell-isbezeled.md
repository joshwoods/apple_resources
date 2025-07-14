

- AppKit
- NSCell
-  isBezeled 

Instance Property

# isBezeled

A Boolean value indicating whether the cell has a bezeled border.

macOS

``` source
@MainActor
var isBezeled: Bool { get set }
```

## Discussion

The value of this property is true if the cell has a bezeled border or false if it does not. This property is mutually exclusive with the isBordered property—that is, a cell’s border can be plain or bezeled but not both. Changing the value of this property automatically removes any border that has been set, regardless of the value you assign to the property.

## See Also

### Managing Display Attributes

var isBordered: Bool

A Boolean value indicating whether the cell draws itself outlined with a plain border.

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

