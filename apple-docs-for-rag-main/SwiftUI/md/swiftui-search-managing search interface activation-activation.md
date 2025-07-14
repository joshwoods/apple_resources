

- SwiftUI
- Search
-  Managing search interface activation 

Article

# Managing search interface activation

Programmatically detect and dismiss a search field.

## Overview

People activate a search field in your app by tapping or clicking it, after which they can enter search terms. In many cases, your app only needs to react to the corresponding changes in the search text values, which the interface updates through the binding that you provide, as described in Performing a search operation.

However, SwiftUI also provides controls that enable you to programmatically manage the search interface. In particular, you can:

- Activate or deactivate the interface using a binding that you provide to the searchable modifier.

- Detect whether the interface is active by reading an environment value.

- Dismiss the interface by calling an action stored in the environment.

- Wait for a search submission event before starting to search.

### Control activation through a binding

You can control search interface activation programmatically by providing the searchable modifier’s `isPresented` parameter with a Binding to a Boolean value. For example, to present a sheet that appears with the search interface already active, create a binding that starts as true:

```
struct SheetView: View {
    @State private var isPresented = true
    @State private var text = ""

    var body: some View {
        NavigationStack {
            SheetContent()
                .searchable(text: $text, isPresented: $isPresented)
        }
    }
}   
```

On iOS and macOS, SwiftUI focuses the search field when presenting search and unfocuses the search field when dismissing search. The search field can also lose focus while the search interface remains presented. For example, if your search interface contains a list of text fields, someone might move focus to one of the text fields without dismissing the interface.

### Detect search activation

If you need to know when the search interface is active, you can query the environment’s isSearching property using the Environment property wrapper. The following example shows a view that updates the text it displays based on the state of the property:

```
struct SearchingExample: View {
    @State private var searchText = ""

    var body: some View {
        NavigationStack {
            SearchedView()
                .searchable(text: $searchText)
        }
    }
}

struct SearchedView: View {
    @Environment(\.isSearching) private var isSearching

    var body: some View {
        Text(isSearching ? "Searching" : "Not searching")
    }
}
```

When someone first taps or clicks in a search field, the `isSearching` property becomes `true`. When they cancel the search operation, the property becomes `false`. It also becomes `false` if you programmatically dismiss the interface, as the next section describes.

Be sure to read the property from inside a view that’s wrapped, either directly or indirectly, by one of the searchable(text:placement:prompt:) view modifiers, like `SearchedView` in the above example. You won’t detect any change in the property value if you read it from outside of that context, like if you put it in the `SearchingExample` view.

### Dismiss the search interface

You can programmatically deactivate the interface using the environment’s dismissSearch action. For example, consider a view with a Button that presents more information about the first matching item from a collection:

```
struct ContentView: View {
    @State private var searchText = ""

    var body: some View {
        NavigationStack {
            SearchedView(searchText: searchText)
                .searchable(text: $searchText)
        }
    }
}

private struct SearchedView: View {
    var searchText: String

    let items = ["a", "b", "c"]
    var filteredItems: [String] { items.filter { $0 == searchText.lowercased() } }

    @State private var isPresented = false
    @Environment(\.dismissSearch) private var dismissSearch

    var body: some View {
        if let item = filteredItems.first {
            Button("Details about \(item)") {
                isPresented = true
            }
            .sheet(isPresented: $isPresented) {
                NavigationStack {
                    DetailView(item: item, dismissSearch: dismissSearch)
                }
            }
        }
    }
}
```

The button becomes visible only after someone enters search text that produces a match. The button’s action shows a sheet that provides more information about the item, including an Add button for adding the item to a stored list of items:

```
private struct DetailView: View {
    var item: String
    var dismissSearch: DismissSearchAction

    @Environment(\.dismiss) private var dismiss

    var body: some View {
        Text("Information about \(item).")
            .toolbar {
                Button("Add") {
                    // Store the item here...

                    dismiss()
                    dismissSearch()
                }
            }
    }
}
```

People can dismiss the sheet by dragging it down, effectively canceling the operation, leaving the in-progress search interaction intact. Alternatively, They can tap the Add button to store the item. Because people are likely done with both the detail view and the search interaction at this point, the button’s closure uses the dismiss property to dismiss the sheet, and the dismissSearch property to reset the search field.

As with the `isSearching` property, be sure to only read `dismissSearch` from within the hierarchy of a searchable view modifier. Calling the action has no effect if you read it from the environment outside of that context. The above example reads the action from `SearchedView`, and passes that into the sheet, because the sheet has its own environment. The action also has no effect if the search interface isn’t active.

### React to search submission

To specify an action that SwiftUI invokes when someone submits the search query (by pressing the Return key), add the onSubmit(of:_:) modifier:

```
SearchedView()
    .searchable(text: $searchText)
    .onSubmit(of: .search) {
        submitCurrentSearchQuery()
    }
```

Depending your app’s structure, you can use search submission in different ways. For example, you can take that opportunity to look for substrings among the search query string that you can convert into tokens. Alternatively, for a search operation that’s very slow, perhaps because it requires a network access, you can wait for a submission event before performing a search.

## See Also

### Detecting, activating, and dismissing search

var isSearching: Bool

A Boolean value that indicates when the user is searching.

var dismissSearch: DismissSearchAction

An action that ends the current search interaction.

struct DismissSearchAction

An action that can end a search interaction.

func searchable(text:isPresented:placement:prompt:)

Marks this view as searchable with programmatic presentation of the search field.

func searchable(text:tokens:isPresented:placement:prompt:token:)

Marks this view as searchable with text and tokens, as well as programmatic presentation.

func searchable(text:editableTokens:isPresented:placement:prompt:token:)

Marks this view as searchable, which configures the display of a search field.

func searchable(text:tokens:suggestedTokens:isPresented:placement:prompt:token:)

Marks this view as searchable with text, tokens, and suggestions, as well as programmatic presentation.

