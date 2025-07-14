

- AppKit
- NSApplication
-  orderFrontStandardAboutPanel(options:) 

Instance Method

# orderFrontStandardAboutPanel(options:)

Displays a standard About window with information from a given options dictionary.

macOS

``` source
@MainActor
func orderFrontStandardAboutPanel(options optionsDictionary: [NSApplication.AboutPanelOptionKey : Any] = [:])
```

## Parameters 

`optionsDictionary`  

A dictionary whose keys define the contents of the About window. For a list of keys, see NSApplication.AboutPanelOptionKey.

## Discussion

In addition to the keys in AboutPanelOptionKey, you may also include the following key in `optionsDictionary`:

- ``` @``"Copyright" ```: An `NSString` object with a line of copyright information. If not specified, this method then looks for the value of `NSHumanReadableCopyright` in the localized version of the app’s `Info.plist` file. If neither is available, this method leaves the space blank.

## See Also

### Managing Panels

func orderFrontColorPanel(Any?)

Brings up the color panel, an instance of `NSColorPanel`.

func orderFrontStandardAboutPanel(Any?)

Displays a standard About window.

func orderFrontCharacterPalette(Any?)

Opens the character palette.

func runPageLayout(Any?)

Displays the receiver’s page layout panel, an instance of `NSPageLayout`.

struct AboutPanelOptionKey

Keys to include in the options dictionary when displaying an About panel.

