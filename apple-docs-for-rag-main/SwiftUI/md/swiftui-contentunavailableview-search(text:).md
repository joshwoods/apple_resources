

- SwiftUI
- ContentUnavailableView
-  search(text:) 

Type Method

# search(text:)

Creates a `ContentUnavailableView` instance that conveys a search state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func search(text: String) -> ContentUnavailableView
```

Available when `Label` is `SearchUnavailableContent.Label`, `Description` is `SearchUnavailableContent.Description`, and `Actions` is `SearchUnavailableContent.Actions`.

## Parameters 

`text`  

The search text query.

## Discussion

For example, consider the usage of this static member in *ContactsListView*:

```
struct ContactsListView: View {
    @ObservedObject private var viewModel = ContactsViewModel()

    var body: some View {
        NavigationStack {
            CustomSearchBar(query: $viewModel.searchText)
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
            .overlay {
                if viewModel.searchResults.isEmpty {
                    ContentUnavailableView
                        .search(text: viewModel.searchText)
                }
            }
        }
    }
}
```

## See Also

### Getting built-in unavailable views

static var search: ContentUnavailableView&lt;SearchUnavailableContent.Label, SearchUnavailableContent.Description, SearchUnavailableContent.Actions>

Creates a `ContentUnavailableView` instance that conveys a search state.

