

- AppKit
- NSFontManager
-  fontPanel(\_:) 

Instance Method

# fontPanel(\_:)

Returns the application’s shared Font panel object, creating it if necessary.

macOS

``` source
func fontPanel(_ create: Bool) -> NSFontPanel?
```

## Parameters 

`create`  

If true, the Font panel object is created if necessary; if false, it is not.

## Return Value

The application’s shared Font panel object.

## See Also

### Related Documentation

class var shared: NSFontPanel

Returns the single `NSFontPanel` instance for the application, creating it if necessary.

class func setFontPanelFactory(AnyClass?)

Sets the class that creates the shared Font panel object.

class var sharedFontPanelExists: Bool

Returns true if the shared Font panel has been created, false if it hasn’t.

### Managing the Font Panel and Font Menu

var isEnabled: Bool

A Boolean value that indicates whether the font conversion system’s Font panel and Font menu items are enabled.

func setFontMenu(NSMenu)

Records the given menu as the application’s Font menu.

func fontMenu(Bool) -> NSMenu?

Returns the menu that’s connected to the font conversion system, creating it if necessary.

