

- SwiftUI
- ControlGroup
-  init(content:) 

Initializer

# init(content:)

Creates a new ControlGroup with the specified children

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
init(@ViewBuilder content: () -> Content)
```

## Parameters 

`content`  

The children to display

## See Also

### Creating a control group

init&lt;C, L>(content: () -> C, label: () -> L)

Creates a new control group with the specified content and a label.

init(_:content:)

Creates a new control group with the specified content that generates its label from a string.

