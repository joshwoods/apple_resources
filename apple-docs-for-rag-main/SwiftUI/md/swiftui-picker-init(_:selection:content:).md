

- SwiftUI
- Picker
-  init(\_:selection:content:) 

Initializer

# init(\_:selection:content:)

Creates a picker that generates its label from a localized string key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    selection: Binding,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Text`, `SelectionValue` conforms to `Hashable`, and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

A localized string key that describes the purpose of selecting an option.

`selection`  

A binding to a property that determines the currently-selected option.

`content`  

A view that contains the set of options.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

## See Also

### Creating a picker

init(selection: Binding&lt;SelectionValue>, content: () -> Content, label: () -> Label)

Creates a picker that displays a custom label.

