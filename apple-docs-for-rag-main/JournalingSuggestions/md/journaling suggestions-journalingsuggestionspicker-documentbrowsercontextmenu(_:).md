

- Journaling Suggestions
- JournalingSuggestionsPicker
-  documentBrowserContextMenu(\_:) 

Instance Method

# documentBrowserContextMenu(\_:)

Adds to a `DocumentLaunchView` actions that accept a list of selected files as their parameter.

Journaling SuggestionsSwiftUIiOS 18.1+

``` source
@MainActor @preconcurrency
func documentBrowserContextMenu(@ViewBuilder _ menu: @escaping ([URL]?) -> some View) -> some View
```

## Parameters 

`menu`  

Items representing the content of the menu.

## Discussion

Add `documentBrowserContextMenu` modifier to `DocumentLaunchView` to provide additional actions to the document browser items’ context menu. For example, a book editor application could have a “Favorite” button that marks user-chosen books as their favorite. The button enables when the user switches the browser into “Selection” mode.

```
import UniformTypeIdentifiers

struct BookEditor: View {

    var body: some View {
        DocumentLaunchView(for: [.book]) {
            NewDocumentButton("Start New Book")
        } onDocumentOpen: { url in
            BookEditor(url)
        }
        .documentBrowserContextMenu { selectedURLs in
            FavoriteBookButton(urls: selectedURLs)
        }
    }
}

struct FavoriteBookButton: View {
    var urls: [URL]?
    var body: some View {
        Button {
            updateFavorite(urls)
        } label: {
            Image(systemName: allFavorite(urls) ? "heart.fill" : "heart")
        }
    }

    func allFavorite(_ urls: [URL]?) -> Bool { ... }
    func updateFavorite(_ urls: [URL]?) { ... }
}

struct BookEditor: View {
    init(_ url: URL) { ... }
}

extension UTType {
    static var book = UTType(exportedAs: "com.example.bookEditor")
}
```

In the example above, the application stores a list of URLs to favorite books, and does not need to access the file on disk. In cases when an application wants to read the contents of the URL from the disk or associated metadata, it should call `URL.startAccessingSecurityScopedResource()` to gain access to the resource, and `URL.stopAccessingSecurityScopedResource()` to relinquish access when it is not needed.

The actions are displayed in the document browser navigation bar when a document browser is in Select mode, and also added to context menu for the file items.

