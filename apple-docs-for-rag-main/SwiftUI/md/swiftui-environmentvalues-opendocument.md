

- SwiftUI
- EnvironmentValues
-  openDocument 

Instance Property

# openDocument

An action in the environment that presents an existing document.

macOS 13.0+

``` source
var openDocument: OpenDocumentAction { get }
```

## Discussion

Use the `openDocument` environment value to get the instance of the OpenDocumentAction structure for a given Environment. Then call the instance to present an existing document. You call the instance directly because it defines a callAsFunction(at:) method that Swift calls when you call the instance.

For example, you can create a button that opens the document at the specified URL:

```
struct OpenDocumentButton: View {
    var url: URL
    @Environment(\.openDocument) private var openDocument

    var body: some View {
        Button(url.deletingPathExtension().lastPathComponent) {
            Task {
                do {
                    try await openDocument(at: url)
                } catch {
                    // Handle error
                }
            }
        }
    }
}
```

The above example uses a `do-catch` statement to handle any errors that the open document action might throw. It also places the action inside a task and awaits the result because the action operates asynchronously.

To present an existing document, your app must define a DocumentGroup that handles the content type of the specified file. For a document that’s already open, the system brings the existing window to the front. Otherwise, the system opens a new window.

## See Also

### Opening a document programmatically

var newDocument: NewDocumentAction

An action in the environment that presents a new document.

struct NewDocumentAction

An action that presents a new document.

struct OpenDocumentAction

An action that presents an existing document.

