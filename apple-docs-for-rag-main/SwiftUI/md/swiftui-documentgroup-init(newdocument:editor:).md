

- SwiftUI
- DocumentGroup
-  init(newDocument:editor:) 

Initializer

# init(newDocument:editor:)

Creates a document group for creating and editing file documents.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@preconcurrency nonisolated
init(
    newDocument: @autoclosure @escaping () -> Document,
    @ViewBuilder editor: @escaping (FileDocumentConfiguration) -> Content
)
```

Available when `Document` conforms to `FileDocument` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`newDocument`  

The initial document to use when a user creates a new document.

`editor`  

The editing UI for the provided document.

## Discussion

Use a DocumentGroup scene to tell SwiftUI what kinds of documents your app can open when you declare your app using the App protocol. You initialize a document group scene by passing in the document model and a view capable of displaying the document’s contents. The document types you supply to DocumentGroup must conform to FileDocument or ReferenceFileDocument. SwiftUI uses the model to add document support to your app. In macOS this includes document-based menu support including the ability to open multiple documents. On iOS this includes a document browser that can navigate to the documents stored on the file system and multiwindow support:

```
@main
struct MyApp: App {
    var body: some Scene {
        DocumentGroup(newDocument: TextFile()) { file in
            ContentView(document: file.$document)
        }
    }
}
```

The document types you supply to DocumentGroup must conform to FileDocument or ReferenceFileDocument. Your app can support multiple document types by adding additional DocumentGroup scenes.

## See Also

### Creating a document group

init(viewing:viewer:)

Creates a document group capable of viewing file documents.

