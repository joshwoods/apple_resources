

- SwiftUI
- LabeledContent
-  init(\_:) 

Initializer

# init(\_:)

Creates labeled content based on a labeled content style configuration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(_ configuration: LabeledContentStyleConfiguration)
```

Available when `Label` is `LabeledContentStyleConfiguration.Label` and `Content` is `LabeledContentStyleConfiguration.Content`.

## Parameters 

`configuration`  

The properties of the labeled content

## Discussion

You can use this initializer within the makeBody(configuration:) method of a LabeledContentStyle to create a labeled content instance. This is useful for custom styles that only modify the current style, as opposed to implementing a brand new style.

For example, the following style adds a red border around the labeled content, but otherwise preserves the current style:

```
struct RedBorderLabeledContentStyle: LabeledContentStyle {
    func makeBody(configuration: Configuration) -> some View {
        LabeledContent(configuration)
            .border(.red)
    }
}
```

## See Also

### Creating labeled content

init(_:content:)

Creates a labeled view that generates its label from a localized string key.

init(content: () -> Content, label: () -> Label)

Creates a standard labeled element, with a view that conveys the value of the element and a label.

init(_:value:)

Creates a labeled informational view.

init(_:value:format:)

Creates a labeled informational view from a formatted value.

