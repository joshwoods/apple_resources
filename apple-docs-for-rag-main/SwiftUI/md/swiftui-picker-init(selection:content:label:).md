

- SwiftUI
- Picker
-  init(selection:content:label:) 

Initializer

# init(selection:content:label:)

Creates a picker that displays a custom label.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(
    selection: Binding,
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View`, `SelectionValue` conforms to `Hashable`, and `Content` conforms to `View`.

## Parameters 

`selection`  

A binding to a property that determines the currently-selected option.

`content`  

A view that contains the set of options.

`label`  

A view that describes the purpose of selecting an option.

## See Also

### Creating a picker

init(_:selection:content:)

Creates a picker that generates its label from a localized string key.

