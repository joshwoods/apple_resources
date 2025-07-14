

- Core Transferable
-  ReceivedTransferredFile 

Structure

# ReceivedTransferredFile

A description of a file from the perspective of the receiver.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ReceivedTransferredFile
```

## Topics

### Configuring a file transfer

let file: URL

The received file on disk.

let isOriginalFile: Bool

A Boolean value that indicates whether the file’s URL points to the original file provided by the sender or to a copy.

## Relationships

### Conforms To

- Sendable

## See Also

### File transfer

struct FileRepresentation

A transfer representation for types that transfer as a file URL.

struct SentTransferredFile

A description of a file from the perspective of the sender.

