

- AppKit
- NSFontManager
-  setFontMenu(\_:) 

Instance Method

# setFontMenu(\_:)

Records the given menu as the application’s Font menu.

macOS

``` source
func setFontMenu(_ newMenu: NSMenu)
```

## Parameters 

`newMenu`  

The new Font menu.

## See Also

### Managing the Font Panel and Font Menu

var isEnabled: Bool

A Boolean value that indicates whether the font conversion system’s Font panel and Font menu items are enabled.

func fontPanel(Bool) -> NSFontPanel?

Returns the application’s shared Font panel object, creating it if necessary.

func fontMenu(Bool) -> NSMenu?

Returns the menu that’s connected to the font conversion system, creating it if necessary.

