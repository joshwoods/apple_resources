

- SwiftUI
- Button
-  init(\_:systemImage:role:action:) 

Initializer

# init(\_:systemImage:role:action:)

Creates a button with a specified role that generates its label from a localized string key and a system image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    systemImage: String,
    role: ButtonRole?,
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

`role`  

An optional semantic role describing the button. A value of `nil` means that the button doesn’t have an assigned role.

`action`  

The action to perform when the user triggers the button.

## Discussion

This initializer creates a Label view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

## See Also

### Creating a button with a role

init(role: ButtonRole?, action: () -> Void, label: () -> Label)

Creates a button with a specified role that displays a custom label.

init(_:role:action:)

Creates a button with a specified role that generates its label from a localized string key.

init(_:image:role:action:)

Creates a button with a specified role that generates its label from a localized string key and an image resource.

