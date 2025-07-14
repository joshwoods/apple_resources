

- SwiftUI
- Button
-  init(\_:systemImage:action:) 

Initializer

# init(\_:systemImage:action:)

Creates a button that generates its label from a localized string key and system image name.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    systemImage: String,
    action: @escaping @MainActor () -> Void
)
```

Available when `Label` is `Label`.

Show all declarations

## Parameters 

`titleKey`  

The key for the button’s localized title, that describes the purpose of the button’s `action`.

`systemImage`  

The name of the image resource to lookup.

`action`  

The action to perform when the user triggers the button.

## Discussion

This initializer creates a Label view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

## See Also

### Creating a button

init(action: () -> Void, label: () -> Label)

Creates a button that displays a custom label.

init(_:action:)

Creates a button that generates its label from a localized string key.

init(_:image:action:)

Creates a button that generates its label from a localized string key and image resource.

