

- SwiftUI
-  ContentUnavailableView 

Structure

# ContentUnavailableView

An interface, consisting of a label and additional content, that you display when the content of your app is unavailable to users.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ContentUnavailableView where Label : View, Description : View, Actions : View
```

## Overview

It is recommended to use `ContentUnavailableView` in situations where a view’s content cannot be displayed. That could be caused by a network error, a list without items, a search that returns no results etc.

You create an `ContentUnavailableView` in its simplest form, by providing a label and some additional content such as a description or a call to action:

```
ContentUnavailableView {
    Label("No Mail", systemImage: "tray.fill")
} description: {
    Text("New mails you receive will appear here.")
}
```

The system provides default `ContentUnavailableView`s that you can use in specific situations. The example below illustrates the usage of the search view:

```
struct ContentView: View {
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

## Topics

### Getting built-in unavailable views

static var search: ContentUnavailableView&lt;SearchUnavailableContent.Label, SearchUnavailableContent.Description, SearchUnavailableContent.Actions>

Creates a `ContentUnavailableView` instance that conveys a search state.

static func search(text: String) -> ContentUnavailableView&lt;Label, Description, Actions>

Creates a `ContentUnavailableView` instance that conveys a search state.

### Creating an unavailable view

init(label: () -> Label, description: () -> Description, actions: () -> Actions)

Creates an interface, consisting of a label and additional content, that you display when the content of your app is unavailable to users.

init(_:image:description:)

Creates an interface, consisting of a title generated from a localized string, an image and additional content, that you display when the content of your app is unavailable to users.

init(_:systemImage:description:)

Creates an interface, consisting of a title generated from a localized string, a system icon image and additional content, that you display when the content of your app is unavailable to users.

### Supporting types

struct SearchUnavailableContent

A structure that represents the body of a static placeholder search view.

## Relationships

### Conforms To

- View

