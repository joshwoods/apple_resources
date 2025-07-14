

- SwiftUI
- FileDocument
-  readableContentTypes 

Type Property

# readableContentTypes

The file and data types that the document reads from.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static var readableContentTypes: [UTType] { get }
```

**Required**

## Discussion

Define this list to indicate the content types that your document can read. By default, SwiftUI assumes that your document can also write the same set of content types. If you need to indicate a different set of types for writing files, define the writableContentTypes property in addition to this property.

## See Also

### Reading a document

init(configuration: Self.ReadConfiguration) throws

Creates a document and initializes it with the contents of a file.

**Required**

typealias ReadConfiguration

The configuration for reading document contents.

