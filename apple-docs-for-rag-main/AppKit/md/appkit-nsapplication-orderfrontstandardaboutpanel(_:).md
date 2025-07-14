

- AppKit
- NSApplication
-  orderFrontStandardAboutPanel(\_:) 

Instance Method

# orderFrontStandardAboutPanel(\_:)

Displays a standard About window.

macOS

``` source
@MainActor
func orderFrontStandardAboutPanel(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the command.

## Discussion

This method calls orderFrontStandardAboutPanel(options:) with a `nil` argument. See orderFrontStandardAboutPanel(options:) for a description of what’s displayed.

## See Also

### Managing Panels

func orderFrontColorPanel(Any?)

Brings up the color panel, an instance of `NSColorPanel`.

func orderFrontStandardAboutPanel(options: [NSApplication.AboutPanelOptionKey : Any])

Displays a standard About window with information from a given options dictionary.

func orderFrontCharacterPalette(Any?)

Opens the character palette.

func runPageLayout(Any?)

Displays the receiver’s page layout panel, an instance of `NSPageLayout`.

struct AboutPanelOptionKey

Keys to include in the options dictionary when displaying an About panel.

