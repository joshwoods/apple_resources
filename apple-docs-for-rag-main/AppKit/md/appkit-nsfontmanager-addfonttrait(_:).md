

- AppKit
- NSFontManager
-  addFontTrait(\_:) 

Instance Method

# addFontTrait(\_:)

Adds a trait to the font.

macOS

``` source
func addFontTrait(_ sender: Any?)
```

## Parameters 

`sender`  

The control that sent the message.

## Discussion

By default, the action message is changeFont:. This action method causes the receiver to send its action message up the responder chain.

When a responder replies by providing a font to convert in a convert(_:) message, the receiver converts the font by adding the trait specified by `sender`. This trait is determined by sending a `tag` message to `sender` and interpreting it as a font trait mask for a convert(_:toHaveTrait:) message.

## See Also

### Sending Action Methods

func removeFontTrait(Any?)

Removes a trait from the font.

func modifyFont(Any?)

Modifies a trait of the font.

func modifyFontViaPanel(Any?)

Modifies a font trait using input from the Font panel.

func orderFrontStylesPanel(Any?)

Opens the Font Styles panel.

func orderFrontFontPanel(Any?)

Opens the Font panel, creating it if necessary, and displays that panel in front of the app’s windows.

enum NSFontAction

Actions that modify a font.

