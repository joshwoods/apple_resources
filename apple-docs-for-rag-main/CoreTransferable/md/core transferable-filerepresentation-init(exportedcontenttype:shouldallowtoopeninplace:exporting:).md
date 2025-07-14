

- Core Transferable
- FileRepresentation
-  init(exportedContentType:shouldAllowToOpenInPlace:exporting:) 

Initializer

# init(exportedContentType:shouldAllowToOpenInPlace:exporting:)

Creates a transfer representation for exporting transferable items as files.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    exportedContentType: UTType,
    shouldAllowToOpenInPlace: Bool = false,
    exporting: @escaping (Item) async throws -> SentTransferredFile
)
```

## Parameters 

`exportedContentType`  

A uniform type identifier for the file `URL`, returned by the `exporting` closure.

`shouldAllowToOpenInPlace`  

A Boolean value that indicates whether the receiver can try to gain access to the original item on disk and can edit it. If `false`, the receiver only has access to a copy of the file made by the system.

`exporting`  

A closure that provides a file representation of the given item.

## See Also

### Creating a transfer representation

init(contentType: UTType, shouldAttemptToOpenInPlace: Bool, exporting: (Item) async throws -> SentTransferredFile, importing: (ReceivedTransferredFile) async throws -> Item)

Creates a transfer representation for importing and exporting transferable items as files.

init(importedContentType: UTType, shouldAttemptToOpenInPlace: Bool, importing: (ReceivedTransferredFile) async throws -> Item)

Creates a transfer representation for importing transferable items as files.

