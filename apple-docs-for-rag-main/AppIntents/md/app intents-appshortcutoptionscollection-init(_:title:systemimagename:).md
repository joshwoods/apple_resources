

- App Intents
- AppShortcutOptionsCollection
-  init(\_:title:systemImageName:) 

Initializer

# init(\_:title:systemImageName:)

Initializes a collection of options for App Shortcuts with the specified parameters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    _ dynamicOptionsProvider: Provider,
    title: LocalizedStringResource,
    systemImageName: String? = nil
)
```

## Parameters 

`dynamicOptionsProvider`  

The object that provides the dynamic options for an App Shortcut.

`title`  

A localized string that represents the title for the collection of dynamic options in the Shortcuts app.

`systemImageName`  

The name of the system image for the collection of App Shortcuts.

