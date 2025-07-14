

- UIKit
-  UITitlebar 

Class

# UITitlebar

An object that you use to configure the title bar of a window in a Mac app built with Mac Catalyst.

Mac Catalyst 13.0+

``` source
@MainActor
class UITitlebar
```

## Overview

Each UIWindowScene has a UITitlebar object available in Mac apps built with Mac Catalyst. You use this object to configure the title bar and its toolbar.

To show or hide a title in the title bar, set the titleVisibility property to UITitlebarTitleVisibility.visible or UITitlebarTitleVisibility.hidden. If you set the visibility to hidden and the title bar’s toolbar property is `nil`, the window displays only the window control buttons (Close, Minimize, and Zoom).

To add a toolbar to a window, create an NSToolbar object and assign it to the title bar’s toolbar property. To automatically hide the toolbar when the window enters full-screen mode, set the autoHidesToolbarInFullScreen property to true.

```
func scene(_ scene: UIScene, willConnectTo session: UISceneSession, options connectionOptions: UIScene.ConnectionOptions) {

    guard let windowScene = (scene as? UIWindowScene) else { return }

    #if targetEnvironment(macCatalyst)
    if  let titlebar = windowScene.titlebar {
        let identifier = NSToolbar.Identifier("com.example.apple-samplecode.toolbar")
        titlebar.toolbar = NSToolbar(identifier: identifier)
        titlebar.toolbar?.delegate = self
        titlebar.autoHidesToolbarInFullScreen = true
    }
    #endif
}
```

## Topics

### Configuring the title bar

var separatorStyle: UITitlebarSeparatorStyle

The type of separator that the app displays between the title bar and content of a window.

enum UITitlebarSeparatorStyle

Styles that determine the type of separator displayed between the title bar and content of a window.

var titleVisibility: UITitlebarTitleVisibility

A value that indicates the visibility of the title.

enum UITitlebarTitleVisibility

States that determine visibility of the title in the title bar.

var representedURL: URL?

A URL of the file or resource represented in the window.

### Configuring the toolbar

var toolbar: NSToolbar?

The toolbar displayed beneath or integrated with the title bar.

var toolbarStyle: UITitlebarToolbarStyle

The style of the toolbar determining its appearance and location related to the title bar.

enum UITitlebarToolbarStyle

Styles that determine the toolbar’s appearance and location related to the title bar.

var autoHidesToolbarInFullScreen: Bool

A Boolean value that determines whether the toolbar automatically hides in full-screen windows.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Configuring a window’s title bar

var titlebar: UITitlebar?

The title bar displayed in a window of a Mac app.

