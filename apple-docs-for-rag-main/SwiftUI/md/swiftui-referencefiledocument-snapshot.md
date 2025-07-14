

- SwiftUI
- ReferenceFileDocument
-  Snapshot 

Associated Type

# Snapshot

A type that represents the document’s stored content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
associatedtype Snapshot
```

**Required**

## Discussion

Define this type to represent all the data that your document stores. When someone issues a Save command, SwiftUI asks your document for a value of this type by calling the document’s snapshot(contentType:) method. SwiftUI sends the snapshot that you provide to the document’s fileWrapper(snapshot:configuration:) method, where you serialize the contents of the snapshot into a file wrapper.

## See Also

### Getting a snapshot

func snapshot(contentType: UTType) throws -> Self.Snapshot

Creates a snapshot that represents the current state of the document.

**Required**

