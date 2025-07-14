

- AppKit
- NSApplication
-  runPageLayout(\_:) 

Instance Method

# runPageLayout(\_:)

Displays the receiver’s page layout panel, an instance of `NSPageLayout`.

macOS

``` source
@MainActor
func runPageLayout(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the command.

## Discussion

If the `NSPageLayout` instance does not exist, this method creates one. This method is typically invoked when the user chooses Page Setup from the app’s File menu.

## See Also

### Managing Panels

func orderFrontColorPanel(Any?)

Brings up the color panel, an instance of `NSColorPanel`.

func orderFrontStandardAboutPanel(Any?)

Displays a standard About window.

func orderFrontStandardAboutPanel(options: [NSApplication.AboutPanelOptionKey : Any])

Displays a standard About window with information from a given options dictionary.

func orderFrontCharacterPalette(Any?)

Opens the character palette.

struct AboutPanelOptionKey

Keys to include in the options dictionary when displaying an About panel.

