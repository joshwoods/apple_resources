

- SwiftUI
-  MenuBarExtra 

Structure

# MenuBarExtra

A scene that renders itself as a persistent control in the system menu bar.

macOS 13.0+

``` source
struct MenuBarExtra where Label : View, Content : View
```

## Overview

Use a `MenuBarExtra` when you want to provide access to commonly used functionality, even when your app is not active.

```
@main
struct AppWithMenuBarExtra: App {
    @AppStorage("showMenuBarExtra") private var showMenuBarExtra = true

    var body: some Scene {
        WindowGroup {
            ContentView()
        }
        MenuBarExtra(
            "App Menu Bar Extra", systemImage: "star",
            isInserted: $showMenuBarExtra)
        {
            StatusMenu()
        }
    }
}
```

Or alternatively, to create a utility app that only shows in the menu bar.

```
@main
struct UtilityApp: App {
    var body: some Scene {
        MenuBarExtra("Utility App", systemImage: "hammer") {
            AppMenu()
        }
    }
}
```

An app that only shows in the menu bar will be automatically terminated if the user removes the extra from the menu bar.

For apps that only show in the menu bar, a common behavior is for the app to not display its icon in either the Dock or the application switcher. To enable this behavior, set the LSUIElement flag in your app’s Information Property List file to `true`.

For more complex or data rich menu bar extras, you can use the window style, which displays a popover-like window from the menu bar icon that contains standard controls. You define the layout and contents of those controls with the content that you provide:

```
MenuBarExtra("Utility App", systemImage: "hammer") {
    ScrollView {
        LazyVGrid(...)
    }
}
.menuBarExtraStyle(.window)
```

## Topics

### Creating a menu bar extra

init(_:content:)

Creates a menu bar extra with a key for a localized string to use as the label. The extra defines the primary scene of an `App`.

init(content: () -> Content, label: () -> Label)

Creates a menu bar extra that will be displayed in the system menu bar, and defines the primary scene of an `App`.

init(_:isInserted:content:)

Creates a menu bar extra with a key for a localized string to use as the label. The item will be displayed in the system menu bar when the specified binding is set to `true`. If the user removes the item from the menu bar, the binding will be set to `false`.

init(isInserted: Binding&lt;Bool>, content: () -> Content, label: () -> Label)

Creates a menu bar extra. The item will be displayed in the system menu bar when the specified binding is set to `true`. If the user removes the item from the menu bar, the binding will be set to `false`.

### Creating a menu bar extra with an image

init(_:image:content:)

Creates a menu bar extra with an image to use as the items label. The provided title will be used by the accessibility system.

init(_:image:isInserted:content:)

Creates a menu bar extra with an image to use as the items label. The provided title will be used by the accessibility system.

init(_:systemImage:content:)

Creates a menu bar extra with a system image to use as the items label. The provided title will be used by the accessibility system.

init(_:systemImage:isInserted:content:)

Creates a menu bar extra with a system image to use as the items label. The provided title will be used by the accessibility system.

## Relationships

### Conforms To

- Scene

## See Also

### Creating a menu bar extra

func menuBarExtraStyle&lt;S>(S) -> some Scene

Sets the style for menu bar extra created by this scene.

protocol MenuBarExtraStyle

A specification for the appearance and behavior of a menu bar extra scene.

