

- SwiftUI
- LabeledContent
-  init(\_:value:) 

Initializer

# init(\_:value:)

Creates a labeled informational view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ title: S1,
    value: S2
) where S1 : StringProtocol, S2 : StringProtocol
```

Available when `Label` is `Text` and `Content` is `Text`.

Show all declarations

## Parameters 

`title`  

A string that describes the purpose of the view.

`value`  

The value being labeled.

## Discussion

This initializer creates a Text label on your behalf, and treats the title similar to init(_:). See `Text` for more information about localizing strings.

```
Form {
    ForEach(person.pet) { pet in
        LabeledContent(pet.species, value: pet.name)
    }
}
```

## See Also

### Creating labeled content

init(_:content:)

Creates a labeled view that generates its label from a localized string key.

init(content: () -> Content, label: () -> Label)

Creates a standard labeled element, with a view that conveys the value of the element and a label.

init(_:value:format:)

Creates a labeled informational view from a formatted value.

init(LabeledContentStyleConfiguration)

Creates labeled content based on a labeled content style configuration.

