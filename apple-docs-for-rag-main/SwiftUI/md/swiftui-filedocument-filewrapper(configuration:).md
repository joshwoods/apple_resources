

- SwiftUI
- FileDocument
-  fileWrapper(configuration:) 

Instance Method

# fileWrapper(configuration:)

Serializes a document snapshot to a file wrapper.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func fileWrapper(configuration: Self.WriteConfiguration) throws -> FileWrapper
```

**Required**

## Parameters 

`configuration`  

Information about a file that already exists for the document, if any.

## Return Value

The destination to serialize the document contents to. The value can be a newly created FileWrapper or an update of the one provided in the `configuration` input.

## Discussion

To store a document — for example, in response to a Save command — SwiftUI calls this method. Use it to serialize the document’s data and create or modify a file wrapper with the serialized data:

```
func fileWrapper(configuration: WriteConfiguration) throws -> FileWrapper {
    let data = try JSONEncoder().encode(model)
    return FileWrapper(regularFileWithContents: data)
}
```

Note

SwiftUI calls this method on a background thread. Don’t make user interface changes from that thread.

## See Also

### Writing a document

static var writableContentTypes: [UTType]

The file types that the document supports saving or exporting to.

**Required** Default implementation provided.

typealias WriteConfiguration

The configuration for writing document contents.

