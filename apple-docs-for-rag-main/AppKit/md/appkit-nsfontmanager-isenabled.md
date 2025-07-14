

- AppKit
- NSFontManager
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the font conversion system’s Font panel and Font menu items are enabled.

macOS

``` source
var isEnabled: Bool { get set }
```

## Discussion

When the value of this property is true, the font conversion system’s user interface items (the Font panel and Font menu items) are enabled; when the value is false, these items are not enabled.

## See Also

### Related Documentation

var isEnabled: Bool

A Boolean that shows whether the receiver’s Set button is enabled.

### Managing the Font Panel and Font Menu

func fontPanel(Bool) -> NSFontPanel?

Returns the application’s shared Font panel object, creating it if necessary.

func setFontMenu(NSMenu)

Records the given menu as the application’s Font menu.

func fontMenu(Bool) -> NSMenu?

Returns the menu that’s connected to the font conversion system, creating it if necessary.

