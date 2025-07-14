

- SwiftUI
- List
-  init(content:) 

Initializer

# init(content:)

Creates a list with the given content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
init(@ViewBuilder content: () -> Content)
```

Available when `SelectionValue` is `Never` and `Content` conforms to `View`.

## Parameters 

`content`  

The content of the list.

## See Also

### Creating a list from a set of views

init(selection:content:)

Creates a list with the given content that supports selecting a single row that cannot be deselcted.

