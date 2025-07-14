

- SwiftUI
- ControlGroup
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a new control group with the specified content that generates its label from a string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
init(
    _ title: S,
    @ViewBuilder content: () -> C
) where Content == LabeledControlGroupContent, C : View, S : StringProtocol
```

Available when `Content` conforms to `View`.

Show all declarations

## Parameters 

`title`  

A string that describes the contents of the group.

## See Also

### Creating a control group

init(content: () -> Content)

Creates a new ControlGroup with the specified children

init&lt;C, L>(content: () -> C, label: () -> L)

Creates a new control group with the specified content and a label.

