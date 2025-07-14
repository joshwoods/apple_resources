

- SwiftUI
- Label
-  init(title:icon:) 

Initializer

# init(title:icon:)

Creates a label with a custom title and icon.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    @ViewBuilder title: () -> Title,
    @ViewBuilder icon: () -> Icon
)
```

## See Also

### Creating a label

init(_:image:)

Creates a label with an icon image and a title generated from a localized string.

init(_:systemImage:)

Creates a label with a system icon image and a title generated from a localized string.

init(_:)

Creates a label representing a family activity application.

init(_:image:)

Creates a label with an icon image and a title generated from a localized string.

