

- SwiftUI
- LabeledContent
-  init(\_:value:format:) 

Initializer

# init(\_:value:format:)

Creates a labeled informational view from a formatted value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ titleKey: LocalizedStringKey,
    value: F.FormatInput,
    format: F
) where F : FormatStyle, F.FormatInput : Equatable, F.FormatOutput == String
```

Available when `Label` is `Text` and `Content` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the view’s localized title, that describes the purpose of the view.

`value`  

The value being labeled.

`format`  

A format style of type `F` to convert the underlying value of type `F.FormatInput` to a string representation.

## Discussion

This initializer creates a Text label on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See `Text` for more information about localizing strings.

```
Form {
    LabeledContent("Age", value: person.age, format: .number)
    LabeledContent("Height", value: person.height,
        format: .measurement(width: .abbreviated))
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

init(LabeledContentStyleConfiguration)

Creates labeled content based on a labeled content style configuration.

