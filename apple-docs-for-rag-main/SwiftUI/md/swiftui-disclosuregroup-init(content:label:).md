

- SwiftUI
- DisclosureGroup
-  init(content:label:) 

Initializer

# init(content:label:)

Creates a disclosure group with the given label and content views.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    @ViewBuilder content: @escaping () -> Content,
    @ViewBuilder label: () -> Label
)
```

## Parameters 

`content`  

The content shown when the disclosure group expands.

`label`  

A view that describes the content of the disclosure group.

## See Also

### Creating a disclosure group

init(_:content:)

Creates a disclosure group, using a provided localized string key to create a text view for the label.

init(_:isExpanded:content:)

Creates a disclosure group, using a provided localized string key to create a text view for the label, and a binding to the expansion state (expanded or collapsed).

init(isExpanded: Binding&lt;Bool>, content: () -> Content, label: () -> Label)

Creates a disclosure group with the given label and content views, and a binding to the expansion state (expanded or collapsed).

