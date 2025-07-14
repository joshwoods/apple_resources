

- UIKit
- UITitlebar
-  toolbarStyle 

Instance Property

# toolbarStyle

The style of the toolbar determining its appearance and location related to the title bar.

Mac Catalyst 14.0+

``` source
@MainActor
var toolbarStyle: UITitlebarToolbarStyle { get set }
```

## Discussion

The default value is UITitlebarToolbarStyle.automatic.

## See Also

### Configuring the toolbar

var toolbar: NSToolbar?

The toolbar displayed beneath or integrated with the title bar.

enum UITitlebarToolbarStyle

Styles that determine the toolbar’s appearance and location related to the title bar.

var autoHidesToolbarInFullScreen: Bool

A Boolean value that determines whether the toolbar automatically hides in full-screen windows.

