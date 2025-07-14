

- SwiftUI
- ControlGroup
-  init(\_:systemImage:content:) 

Initializer

# init(\_:systemImage:content:)

Creates a new control group with the specified content that generates its label from a string and image name.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(
    _ title: S,
    systemImage: String,
    @ViewBuilder content: () -> C
) where Content == LabeledControlGroupContent>, C : View, S : StringProtocol
```

Available when `Content` conforms to `View`.

Show all declarations

## Parameters 

`title`  

A string that describes the contents of the group.

`systemImage`  

The name of the image resource to lookup.

## See Also

### Creating a control group with an image

init(_:image:content:)

Creates a new control group with the specified content that generates its label from a string and image name.

