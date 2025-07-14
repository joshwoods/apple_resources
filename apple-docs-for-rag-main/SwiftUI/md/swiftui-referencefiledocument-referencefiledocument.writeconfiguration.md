

- SwiftUI
- ReferenceFileDocument
-  ReferenceFileDocument.WriteConfiguration 

Type Alias

# ReferenceFileDocument.WriteConfiguration

The configuration for writing document contents.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
typealias WriteConfiguration = FileDocumentWriteConfiguration
```

## Discussion

This type is an alias for FileDocumentWriteConfiguration, which contains a content type and a file wrapper that you use to access the contents of a document file, if one already exists. You get a value of this type as an input to the fileWrapper(snapshot:configuration:) method.

## See Also

### Writing a document

func fileWrapper(snapshot: Self.Snapshot, configuration: Self.WriteConfiguration) throws -> FileWrapper

Serializes a document snapshot to a file wrapper.

**Required**

static var writableContentTypes: [UTType]

The file types that the document supports saving or exporting to.

**Required** Default implementation provided.

