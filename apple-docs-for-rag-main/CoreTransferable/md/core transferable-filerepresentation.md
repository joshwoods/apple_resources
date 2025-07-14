

- Core Transferable
-  FileRepresentation 

Structure

# FileRepresentation

A transfer representation for types that transfer as a file URL.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct FileRepresentation where Item : Transferable
```

## Mentioned in 

Choosing a transfer representation for a model type

## Overview

Use a FileRepresentation for transferring types that involve a large amount of data. For example, if your app defines a `Movie` type that could represent a lengthy video, use a `FileRepresentation` instance to transfer the video data to another app or process.

```
struct Movie: Transferable {
    let url: URL
    static var transferRepresentation: some TransferRepresentation {
        FileRepresentation(contentType: .mpeg4Movie) { movie in
            SentTransferredFile($0.url)
            } importing: { received in
                let copy: URL = URL(fileURLWithPath: "")
                try FileManager.default.copyItem(at: received.file, to: copy)
                return Self.init(url: copy) }
    }
}
```

It’s efficient to pass such data around as a file and the receiver loads it into memory only if it’s required.

## Topics

### Creating a transfer representation

init(contentType: UTType, shouldAttemptToOpenInPlace: Bool, exporting: (Item) async throws -> SentTransferredFile, importing: (ReceivedTransferredFile) async throws -> Item)

Creates a transfer representation for importing and exporting transferable items as files.

init(importedContentType: UTType, shouldAttemptToOpenInPlace: Bool, importing: (ReceivedTransferredFile) async throws -> Item)

Creates a transfer representation for importing transferable items as files.

init(exportedContentType: UTType, shouldAllowToOpenInPlace: Bool, exporting: (Item) async throws -> SentTransferredFile)

Creates a transfer representation for exporting transferable items as files.

### Type Aliases

typealias Body

The transfer representation for the item.

### Default Implementations

TransferRepresentation Implementations

## Relationships

### Conforms To

- Sendable
- TransferRepresentation

## See Also

### File transfer

struct SentTransferredFile

A description of a file from the perspective of the sender.

struct ReceivedTransferredFile

A description of a file from the perspective of the receiver.

