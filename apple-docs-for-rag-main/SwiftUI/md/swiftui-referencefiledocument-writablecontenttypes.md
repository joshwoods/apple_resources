

- SwiftUI
- ReferenceFileDocument
-  writableContentTypes 

Type Property

# writableContentTypes

The file types that the document supports saving or exporting to.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static var writableContentTypes: [UTType] { get }
```

**Required** Default implementation provided.

## Discussion

By default, SwiftUI assumes that your document reads and writes the same set of content types. Only define this property if you need to indicate a different set of types for writing files. Otherwise, the default implementation of this property returns the list that you specify in your implementation of readableContentTypes.

## Default Implementations

### ReferenceFileDocument Implementations

static var writableContentTypes: [UTType]

The file types that the document supports saving or exporting to.

## See Also

### Writing a document

func fileWrapper(snapshot: Self.Snapshot, configuration: Self.WriteConfiguration) throws -> FileWrapper

Serializes a document snapshot to a file wrapper.

**Required**

typealias WriteConfiguration

The configuration for writing document contents.

