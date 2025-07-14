

- SwiftUI
- ContentUnavailableView
-  init(\_:image:description:) 

Initializer

# init(\_:image:description:)

Creates an interface, consisting of a title generated from a localized string, an image and additional content, that you display when the content of your app is unavailable to users.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    _ title: LocalizedStringKey,
    image name: String,
    description: Text? = nil
)
```

Available when `Label` is `Label`, `Description` is `Text?`, and `Actions` is `EmptyView`.

Show all declarations

## Parameters 

`title`  

A title generated from a localized string.

`description`  

The view that describes the interface.

## See Also

### Creating an unavailable view

init(label: () -> Label, description: () -> Description, actions: () -> Actions)

Creates an interface, consisting of a label and additional content, that you display when the content of your app is unavailable to users.

init(_:systemImage:description:)

Creates an interface, consisting of a title generated from a localized string, a system icon image and additional content, that you display when the content of your app is unavailable to users.

