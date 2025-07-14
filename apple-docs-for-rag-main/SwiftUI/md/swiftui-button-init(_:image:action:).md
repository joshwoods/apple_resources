

- SwiftUI
- Button
-  init(\_:image:action:) 

Initializer

# init(\_:image:action:)

Creates a button that generates its label from a localized string key and image resource.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@preconcurrency nonisolated
init(
    _ titleKey: LocalizedStringKey,
    image: ImageResource,
    action: @escaping @MainActor () -> Void
)
```

Available when `Label` is `Label`.

Show all declarations

## Parameters 

`titleKey`  

The key for the button’s localized title, that describes the purpose of the button’s `action`.

`image`  

The image resource to lookup.

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

init(_:systemImage:action:)

Creates a button that generates its label from a localized string key and system image name.

