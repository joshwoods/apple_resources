

- RealityKit
- ObjectCaptureView
-  searchPresentationToolbarBehavior(\_:) 

Instance Method

# searchPresentationToolbarBehavior(\_:)

Configures the search toolbar presentation behavior for any searchable modifiers within this view.

RealityKitSwiftUIiOS 17.1+iPadOS 17.1+macOS 14.1+tvOS 17.1+watchOS 10.1+

``` source
nonisolated
func searchPresentationToolbarBehavior(_ behavior: SearchPresentationToolbarBehavior) -> some View
```

## Discussion

By default on iOS, a toolbar may hide parts of its content when presenting search to focus on searching. You can override this behavior by providing a value of `SearchPresentationToolbarBehavior/avoidHidingContent` to this modifer.

```
@State private var searchText = ""

List {
    // ... content
}
.searchable(text: $searchText)
.searchPresentationToolbarBehavior(.avoidHidingContent)
```

