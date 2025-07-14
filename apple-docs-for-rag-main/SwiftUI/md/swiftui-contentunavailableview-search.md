

- SwiftUI
- ContentUnavailableView
-  search 

Type Property

# search

Creates a `ContentUnavailableView` instance that conveys a search state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var search: ContentUnavailableView { get }
```

Available when `Label` is `SearchUnavailableContent.Label`, `Description` is `SearchUnavailableContent.Description`, and `Actions` is `SearchUnavailableContent.Actions`.

## Discussion

A `ContentUnavailableView` initialized with this static member is expected to be contained within a searchable view hierarchy. Such a configuration enables the search query to be parsed into the view’s description.

For example, consider the usage of this static member in *ContactsListView*:

```
struct ContactsListView: View {
    @ObservedObject private var viewModel = ContactsViewModel()

    var body: some View {
        NavigationStack {
            List {
                ForEach(viewModel.searchResults) { contact in
                    NavigationLink {
                        ContactsView(contact)
                    } label: {
                        Text(contact.name)
                    }
                }
            }
            .navigationTitle("Contacts")
            .searchable(text: $viewModel.searchText)
            .overlay {
                if searchResults.isEmpty {
                    ContentUnavailableView.search
                }
            }
        }
    }
}
```

## See Also

### Getting built-in unavailable views

static func search(text: String) -> ContentUnavailableView&lt;Label, Description, Actions>

Creates a `ContentUnavailableView` instance that conveys a search state.

