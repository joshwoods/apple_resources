

- SwiftUI
- List
-  init(selection:content:) 

Initializer

# init(selection:content:)

Creates a list with the given content that supports selecting a single row that cannot be deselcted.

macOS 13.0+

``` source
@MainActor @preconcurrency
init(
    selection: Binding,
    @ViewBuilder content: () -> Content
)
```

Show all declarations

## Parameters 

`selection`  

A binding to a selected row.

`content`  

The content of the list.

## See Also

### Creating a list from a set of views

init(content: () -> Content)

Creates a list with the given content.

