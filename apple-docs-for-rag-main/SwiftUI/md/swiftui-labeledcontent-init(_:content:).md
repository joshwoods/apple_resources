

- SwiftUI
- LabeledContent
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates a labeled view that generates its label from a localized string key.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Text` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

The key for the view’s localized title, that describes the purpose of the view.

`content`  

The value content being labeled.

## Discussion

This initializer creates a Text label on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See `Text` for more information about localizing strings.

## See Also

### Creating labeled content

init(content: () -> Content, label: () -> Label)

Creates a standard labeled element, with a view that conveys the value of the element and a label.

init(_:value:)

Creates a labeled informational view.

init(_:value:format:)

Creates a labeled informational view from a formatted value.

init(LabeledContentStyleConfiguration)

Creates labeled content based on a labeled content style configuration.

