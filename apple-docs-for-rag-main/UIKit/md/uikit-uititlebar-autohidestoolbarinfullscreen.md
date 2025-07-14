

- UIKit
- UITitlebar
-  autoHidesToolbarInFullScreen 

Instance Property

# autoHidesToolbarInFullScreen

A Boolean value that determines whether the toolbar automatically hides in full-screen windows.

Mac Catalyst 13.0+

``` source
@MainActor
var autoHidesToolbarInFullScreen: Bool { get set }
```

## Discussion

Set this property to true to automatically hide the toolbar when the window enters full-screen mode. While hidden, the user can view the toolbar and menu bar by moving the pointer to the top of the screen. Moving the pointer away from the top of the screen hides the toolbar and menu bar.

The default value is false.

## See Also

### Configuring the toolbar

var toolbar: NSToolbar?

The toolbar displayed beneath or integrated with the title bar.

var toolbarStyle: UITitlebarToolbarStyle

The style of the toolbar determining its appearance and location related to the title bar.

enum UITitlebarToolbarStyle

Styles that determine the toolbar’s appearance and location related to the title bar.

