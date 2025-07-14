

- AppKit
- NSFontManager
-  modifyFont(\_:) 

Instance Method

# modifyFont(\_:)

Modifies a trait of the font.

macOS

``` source
func modifyFont(_ sender: Any?)
```

## Parameters 

`sender`  

The control that sent the message.

## Discussion

By default, the action message is changeFont:. This action method causes the receiver to send its action message up the responder chain.

When a responder replies by providing a font to convert in a convert(_:) message, the receiver converts the font in the manner specified by `sender`. The conversion is determined by sending a `tag` message to `sender` and invoking a corresponding method:

| Sender’s Tag | Method Used |
|----|----|
| `NSNoFontChangeAction` | None; the font is returned unchanged. |
| `NSViaPanelFontAction` | The Font panel’s convert(_:). |
| `NSAddTraitFontAction` | convert(_:toHaveTrait:). |
| `NSRemoveTraitFontAction` | convert(_:toNotHaveTrait:). |
| `NSSizeUpFontAction` | convert(_:toSize:). |
| `NSSizeDownFontAction` | convert(_:toSize:). |
| `NSHeavierFontAction` | convertWeight(_:of:). |
| `NSLighterFontAction` | convertWeight(_:of:). |

## See Also

### Sending Action Methods

func addFontTrait(Any?)

Adds a trait to the font.

func removeFontTrait(Any?)

Removes a trait from the font.

func modifyFontViaPanel(Any?)

Modifies a font trait using input from the Font panel.

func orderFrontStylesPanel(Any?)

Opens the Font Styles panel.

func orderFrontFontPanel(Any?)

Opens the Font panel, creating it if necessary, and displays that panel in front of the app’s windows.

enum NSFontAction

Actions that modify a font.

