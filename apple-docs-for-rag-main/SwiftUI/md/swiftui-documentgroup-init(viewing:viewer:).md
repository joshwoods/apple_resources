

- SwiftUI
- DocumentGroup
-  init(viewing:viewer:) 

Initializer

# init(viewing:viewer:)

Creates a document group capable of viewing file documents.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
nonisolated
init(
    viewing documentType: Document.Type,
    @ViewBuilder viewer: @escaping (FileDocumentConfiguration) -> Content
)
```

Available when `Document` conforms to `FileDocument` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`documentType`  

The type of document your app can view.

`viewer`  

The viewing UI for the provided document.

## Discussion

Use this method to create a document group that can view files of a specific type. The example below creates a new document viewer for `MyImageFormatDocument` and displays them with `MyImageFormatViewer`:

```
@main
struct MyApp: App {
    var body: some Scene {
        DocumentGroup(viewing: MyImageFormatDocument.self) { file in
            MyImageFormatViewer(image: file.document)
        }
    }
}
```

You tell the system about the app’s role with respect to the document type by setting the CFBundleTypeRole `Info.plist` key with a value of `Viewer`.

## See Also

### Creating a document group

init(newDocument:editor:)

Creates a document group for creating and editing file documents.

