

- AppKit
- NSApplication
-  orderFrontColorPanel(\_:) 

Instance Method

# orderFrontColorPanel(\_:)

Brings up the color panel, an instance of `NSColorPanel`.

macOS

``` source
@MainActor
func orderFrontColorPanel(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the command.

## Discussion

If the `NSColorPanel` object does not exist yet, this method creates one. This method is typically invoked when the user chooses Colors from a menu.

## See Also

### Managing Panels

func orderFrontStandardAboutPanel(Any?)

Displays a standard About window.

func orderFrontStandardAboutPanel(options: [NSApplication.AboutPanelOptionKey : Any])

Displays a standard About window with information from a given options dictionary.

func orderFrontCharacterPalette(Any?)

Opens the character palette.

func runPageLayout(Any?)

Displays the receiver’s page layout panel, an instance of `NSPageLayout`.

struct AboutPanelOptionKey

Keys to include in the options dictionary when displaying an About panel.

