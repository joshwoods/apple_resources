

- SwiftUI
- ReferenceFileDocument
-  ReferenceFileDocument.ReadConfiguration 

Type Alias

# ReferenceFileDocument.ReadConfiguration

The configuration for reading document contents.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
typealias ReadConfiguration = FileDocumentReadConfiguration
```

## Discussion

This type is an alias for FileDocumentReadConfiguration, which contains a content type and a file wrapper that you use to access the contents of a document file. You get a value of this type as an input to the init(configuration:) initializer. Use it to load a document from a file.

## See Also

### Reading a document

init(configuration: Self.ReadConfiguration) throws

Creates a document and initializes it with the contents of a file.

**Required**

static var readableContentTypes: [UTType]

The file and data types that the document reads from.

**Required**

