

- SwiftUI
- LabeledContent
-  init(content:label:) 

Initializer

# init(content:label:)

Creates a standard labeled element, with a view that conveys the value of the element and a label.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View` and `Content` conforms to `View`.

## Parameters 

`content`  

The view that conveys the value of the resulting labeled element.

`label`  

The label that describes the purpose of the result.

## See Also

### Creating labeled content

init(_:content:)

Creates a labeled view that generates its label from a localized string key.

init(_:value:)

Creates a labeled informational view.

init(_:value:format:)

Creates a labeled informational view from a formatted value.

init(LabeledContentStyleConfiguration)

Creates labeled content based on a labeled content style configuration.

