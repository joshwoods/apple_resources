

- AppKit
- NSApplication
-  orderFrontCharacterPalette(\_:) 

Instance Method

# orderFrontCharacterPalette(\_:)

Opens the character palette.

macOS

``` source
@MainActor
func orderFrontCharacterPalette(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the command.

## See Also

### Managing Panels

func orderFrontColorPanel(Any?)

Brings up the color panel, an instance of `NSColorPanel`.

func orderFrontStandardAboutPanel(Any?)

Displays a standard About window.

func orderFrontStandardAboutPanel(options: [NSApplication.AboutPanelOptionKey : Any])

Displays a standard About window with information from a given options dictionary.

func runPageLayout(Any?)

Displays the receiver’s page layout panel, an instance of `NSPageLayout`.

struct AboutPanelOptionKey

Keys to include in the options dictionary when displaying an About panel.

