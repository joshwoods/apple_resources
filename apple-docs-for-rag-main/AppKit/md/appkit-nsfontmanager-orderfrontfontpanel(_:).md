

- AppKit
- NSFontManager
-  orderFrontFontPanel(\_:) 

Instance Method

# orderFrontFontPanel(\_:)

Opens the Font panel, creating it if necessary, and displays that panel in front of the app’s windows.

macOS

``` source
func orderFrontFontPanel(_ sender: Any?)
```

## Parameters 

`sender`  

The control that sent the message.

## See Also

### Related Documentation

func fontPanel(Bool) -> NSFontPanel?

Returns the application’s shared Font panel object, creating it if necessary.

class func setFontPanelFactory(AnyClass?)

Sets the class that creates the shared Font panel object.

### Sending Action Methods

func addFontTrait(Any?)

Adds a trait to the font.

func removeFontTrait(Any?)

Removes a trait from the font.

func modifyFont(Any?)

Modifies a trait of the font.

func modifyFontViaPanel(Any?)

Modifies a font trait using input from the Font panel.

func orderFrontStylesPanel(Any?)

Opens the Font Styles panel.

enum NSFontAction

Actions that modify a font.

