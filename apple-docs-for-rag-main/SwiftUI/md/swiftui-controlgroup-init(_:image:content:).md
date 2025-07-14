

- SwiftUI
- ControlGroup
-  init(\_:image:content:) 

Initializer

# init(\_:image:content:)

Creates a new control group with the specified content that generates its label from a string and image name.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(
    _ title: S,
    image: ImageResource,
    @ViewBuilder content: () -> C
) where Content == LabeledControlGroupContent>, C : View, S : StringProtocol
```

Available when `Content` conforms to `View`.

Show all declarations

## Parameters 

`title`  

A string that describes the contents of the group.

## See Also

### Creating a control group with an image

init(_:systemImage:content:)

Creates a new control group with the specified content that generates its label from a string and image name.

