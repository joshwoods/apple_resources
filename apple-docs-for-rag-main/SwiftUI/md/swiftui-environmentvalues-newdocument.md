

- SwiftUI
- EnvironmentValues
-  newDocument 

Instance Property

# newDocument

An action in the environment that presents a new document.

macOS 13.0+

``` source
var newDocument: NewDocumentAction { get }
```

## Discussion

Use the `newDocument` environment value to get the instance of the NewDocumentAction structure for a given Environment. Then call the instance to present a new document. You call the instance directly because it defines a callAsFunction(_:) method that Swift calls when you call the instance.

For example, you can define a button that creates a new document from the selected text:

```
struct NewDocumentFromSelection: View {
    @FocusedBinding(\.selectedText) private var selectedText: String?
    @Environment(\.newDocument) private var newDocument

    var body: some View {
        Button("New Document With Selection") {
            newDocument(TextDocument(text: selectedText))
        }
        .disabled(selectedText?.isEmpty != false)
    }
}
```

The above example assumes that you define a `TextDocument` that conforms to the FileDocument or ReferenceFileDocument protocol, and a DocumentGroup that handles the associated file type.

## See Also

### Opening a document programmatically

struct NewDocumentAction

An action that presents a new document.

var openDocument: OpenDocumentAction

An action in the environment that presents an existing document.

struct OpenDocumentAction

An action that presents an existing document.

