

- AppKit
- NSFontManager
-  fontMenu(\_:) 

Instance Method

# fontMenu(\_:)

Returns the menu that’s connected to the font conversion system, creating it if necessary.

macOS

``` source
func fontMenu(_ create: Bool) -> NSMenu?
```

## Parameters 

`create`  

If true, the menu object is created if necessary; if false, it is not.

## Return Value

The font conversion system menu.

## See Also

### Managing the Font Panel and Font Menu

var isEnabled: Bool

A Boolean value that indicates whether the font conversion system’s Font panel and Font menu items are enabled.

func fontPanel(Bool) -> NSFontPanel?

Returns the application’s shared Font panel object, creating it if necessary.

func setFontMenu(NSMenu)

Records the given menu as the application’s Font menu.

