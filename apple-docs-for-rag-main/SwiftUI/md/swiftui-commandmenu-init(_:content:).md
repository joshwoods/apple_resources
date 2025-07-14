

- SwiftUI
- CommandMenu
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a new menu for a collection of app-specific commands, inserted in the standard location for app menus (after the View menu, in order with other menus declared without an explicit location).

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    _ name: Text,
    @ViewBuilder content: () -> Content
)
```

Show all declarations

