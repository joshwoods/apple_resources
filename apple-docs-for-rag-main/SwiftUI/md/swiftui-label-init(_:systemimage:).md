

- SwiftUI
- Label
-  init(\_:systemImage:) 

Initializer

# init(\_:systemImage:)

Creates a label with a system icon image and a title generated from a localized string.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    systemImage name: String
)
```

Available when `Title` is `Text` and `Icon` is `Image`.

Show all declarations

## Parameters 

`titleKey`  

A title generated from a localized string.

## See Also

### Creating a label

init(_:image:)

Creates a label with an icon image and a title generated from a localized string.

init(title: () -> Title, icon: () -> Icon)

Creates a label with a custom title and icon.

init(_:)

Creates a label representing a family activity application.

init(_:image:)

Creates a label with an icon image and a title generated from a localized string.

