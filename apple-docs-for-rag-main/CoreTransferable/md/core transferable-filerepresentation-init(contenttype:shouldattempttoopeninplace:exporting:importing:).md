

- Core Transferable
- FileRepresentation
-  init(contentType:shouldAttemptToOpenInPlace:exporting:importing:) 

Initializer

# init(contentType:shouldAttemptToOpenInPlace:exporting:importing:)

Creates a transfer representation for importing and exporting transferable items as files.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    contentType: UTType,
    shouldAttemptToOpenInPlace: Bool = false,
    exporting: @escaping (Item) async throws -> SentTransferredFile,
    importing: @escaping (ReceivedTransferredFile) async throws -> Item
)
```

## Parameters 

`contentType`  

A uniform type identifier that best describes the item.

`shouldAttemptToOpenInPlace`  

A Boolean value that indicates whether the receiver gains access to the original item on disk and can edit it, or to a copy made by the system.

`exporting`  

A closure that provides a file representation of the given item.

`importing`  

A closure that instantiates the item with given file promise. The file referred to by the file property of the ReceivedTransferredFile instance is only guaranteed to exist within the `importing` closure. If you need the file to be around for a longer period, make a copy in the `importing` closure.

## See Also

### Creating a transfer representation

init(importedContentType: UTType, shouldAttemptToOpenInPlace: Bool, importing: (ReceivedTransferredFile) async throws -> Item)

Creates a transfer representation for importing transferable items as files.

init(exportedContentType: UTType, shouldAllowToOpenInPlace: Bool, exporting: (Item) async throws -> SentTransferredFile)

Creates a transfer representation for exporting transferable items as files.

