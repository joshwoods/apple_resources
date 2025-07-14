

- SwiftUI
- ContentUnavailableView
-  init(label:description:actions:) 

Initializer

# init(label:description:actions:)

Creates an interface, consisting of a label and additional content, that you display when the content of your app is unavailable to users.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    @ViewBuilder label: () -> Label,
    @ViewBuilder description: () -> Description = { EmptyView() },
    @ViewBuilder actions: () -> Actions = { EmptyView() }
)
```

## Parameters 

`label`  

The label that describes the view.

`description`  

The view that describes the interface.

`actions`  

The content of the interface actions.

## See Also

### Creating an unavailable view

init(_:image:description:)

Creates an interface, consisting of a title generated from a localized string, an image and additional content, that you display when the content of your app is unavailable to users.

init(_:systemImage:description:)

Creates an interface, consisting of a title generated from a localized string, a system icon image and additional content, that you display when the content of your app is unavailable to users.

