

- SwiftUI
- View
-  searchPresentationToolbarBehavior(\_:) 

Instance Method

# searchPresentationToolbarBehavior(\_:)

Configures the search toolbar presentation behavior for any searchable modifiers within this view.

iOS 17.1+iPadOS 17.1+Mac Catalyst 17.1+macOS 14.1+tvOS 17.1+visionOS 1.0+watchOS 10.1+

``` source
nonisolated
func searchPresentationToolbarBehavior(_ behavior: SearchPresentationToolbarBehavior) -> some View
```

## Discussion

By default on iOS, a toolbar may hide parts of its content when presenting search to focus on searching. You can override this behavior by providing a value of avoidHidingContent to this modifer.

```
@State private var searchText = ""

List {
    // ... content
}
.searchable(text: $searchText)
.searchPresentationToolbarBehavior(.avoidHidingContent)
```

## See Also

### Displaying toolbar content during search

struct SearchPresentationToolbarBehavior

A type that defines how the toolbar behaves when presenting search.

