

- SwiftUI
- FileDocument
-  init(configuration:) 

Initializer

# init(configuration:)

Creates a document and initializes it with the contents of a file.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(configuration: Self.ReadConfiguration) throws
```

**Required**

## Parameters 

`configuration`  

Information about the file that you read document data from.

## Discussion

SwiftUI calls this initializer when someone opens a file type that matches one of those that your document type supports. Use the file property of the `configuration` input to get document’s data. Deserialize the data, and store it in your document’s data structure:

```
init(configuration: ReadConfiguration) throws {
    guard let data = configuration.file.regularFileContents
    else { /* Throw an error. */ }
    model = try JSONDecoder().decode(Model.self, from: data)
}
```

The above example assumes that you define `Model` to contain the document’s data, that `Model` conforms to the Codable protocol, and that you store a `model` property of that type inside your document.

Note

SwiftUI calls this method on a background thread. Don’t make user interface changes from that thread.

## See Also

### Reading a document

static var readableContentTypes: [UTType]

The file and data types that the document reads from.

**Required**

typealias ReadConfiguration

The configuration for reading document contents.

