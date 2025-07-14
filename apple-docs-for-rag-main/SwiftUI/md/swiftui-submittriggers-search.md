

- SwiftUI
- SubmitTriggers
-  search 

Type Property

# search

Defines triggers originating from search fields constructed from searchable modifiers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let search: SubmitTriggers
```

## Discussion

In the example below, only the search field or search completions placed by the searchable modifier will trigger the view model to submit its current search query.

```
@StateObject private var viewModel = ViewModel()

NavigationView {
    SidebarView()
    DetailView()
}
.searchable(
    text: $viewModel.searchText,
    placement: .sidebar
) {
    SuggestionsView()
}
.onSubmit(of: .search) {
    viewModel.submitCurrentSearchQuery()
}
```

## See Also

### Getting submit triggers

static let text: SubmitTriggers

Defines triggers originating from text input controls like `TextField` and `SecureField`.

