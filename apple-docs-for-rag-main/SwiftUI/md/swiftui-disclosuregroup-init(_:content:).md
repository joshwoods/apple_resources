

- SwiftUI
- DisclosureGroup
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a disclosure group, using a provided localized string key to create a text view for the label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder content: @escaping () -> Content
)
```

Available when `Label` is `Text` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized label of `self` that describes the content of the disclosure group.

`content`  

The content shown when the disclosure group expands.

## See Also

### Creating a disclosure group

init(content: () -> Content, label: () -> Label)

Creates a disclosure group with the given label and content views.

init(_:isExpanded:content:)

Creates a disclosure group, using a provided localized string key to create a text view for the label, and a binding to the expansion state (expanded or collapsed).

init(isExpanded: Binding&lt;Bool>, content: () -> Content, label: () -> Label)

Creates a disclosure group with the given label and content views, and a binding to the expansion state (expanded or collapsed).

