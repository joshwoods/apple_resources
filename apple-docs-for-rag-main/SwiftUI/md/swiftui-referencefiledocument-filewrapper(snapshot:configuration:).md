

- SwiftUI
- ReferenceFileDocument
-  fileWrapper(snapshot:configuration:) 

Instance Method

# fileWrapper(snapshot:configuration:)

Serializes a document snapshot to a file wrapper.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func fileWrapper(
    snapshot: Self.Snapshot,
    configuration: Self.WriteConfiguration
) throws -> FileWrapper
```

**Required**

## Parameters 

`snapshot`  

The document snapshot to save.

`configuration`  

Information about a file that already exists for the document, if any.

## Return Value

The destination to serialize the document contents to. The value can be a newly created FileWrapper or an update of the one provided in the `configuration` input.

## Discussion

To store a document — for example, in response to a Save command — SwiftUI begins by calling the snapshot(contentType:) method to get a copy of the document data in its current state. Then SwiftUI passes that snapshot to this method, where you serialize it and create or modify a file wrapper with the serialized data:

```
func fileWrapper(snapshot: Snapshot, configuration: WriteConfiguration) throws -> FileWrapper {
    let data = try JSONEncoder().encode(snapshot)
    return FileWrapper(regularFileWithContents: data)
}
```

SwiftUI disables document edits during the snapshot to ensure that the document’s data remains coherent, but reenables edits during the serialization operation.

Note

SwiftUI calls this method on a background thread. Don’t make user interface changes from that thread.

## See Also

### Writing a document

static var writableContentTypes: [UTType]

The file types that the document supports saving or exporting to.

**Required** Default implementation provided.

typealias WriteConfiguration

The configuration for writing document contents.

