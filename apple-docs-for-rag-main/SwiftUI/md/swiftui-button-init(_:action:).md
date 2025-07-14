

- SwiftUI
- Button
-  init(\_:action:) 

Initializer

# init(\_:action:)

Creates a button that generates its label from a localized string key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency nonisolated
init(
    _ titleKey: LocalizedStringKey,
    action: @escaping @MainActor () -> Void
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the button’s localized title, that describes the purpose of the button’s `action`.

`action`  

The action to perform when the user triggers the button.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

## See Also

### Creating a button

init(action: () -> Void, label: () -> Label)

Creates a button that displays a custom label.

init(_:image:action:)

Creates a button that generates its label from a localized string key and image resource.

init(_:systemImage:action:)

Creates a button that generates its label from a localized string key and system image name.

