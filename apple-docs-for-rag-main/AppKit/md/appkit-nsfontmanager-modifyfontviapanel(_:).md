

- AppKit
- NSFontManager
-  modifyFontViaPanel(\_:) 

Instance Method

# modifyFontViaPanel(\_:)

Modifies a font trait using input from the Font panel.

macOS

``` source
func modifyFontViaPanel(_ sender: Any?)
```

## Parameters 

`sender`  

The control that sent the message.

## Discussion

By default, the action message is changeFont:. This action method causes the receiver to send its action message up the responder chain.

When a responder replies by providing a font to convert in a convert(_:) message, the receiver converts the font by sending a convert(_:) message to the Font panel. The panel in turn may send convert(_:toFamily:), convert(_:toHaveTrait:), and other specific conversion methods to make its change.

## See Also

### Sending Action Methods

func addFontTrait(Any?)

Adds a trait to the font.

func removeFontTrait(Any?)

Removes a trait from the font.

func modifyFont(Any?)

Modifies a trait of the font.

func orderFrontStylesPanel(Any?)

Opens the Font Styles panel.

func orderFrontFontPanel(Any?)

Opens the Font panel, creating it if necessary, and displays that panel in front of the app’s windows.

enum NSFontAction

Actions that modify a font.

