

- CloudKit
- CKShareTransferRepresentation
-  CKShareTransferRepresentation.ExportedShare 

Structure

# CKShareTransferRepresentation.ExportedShare

An intermediate structure that returns an existing share or prepares a new one if it doesn’t exist.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS

``` source
struct ExportedShare
```

## Topics

### Preparing an exported share

static func existing(CKShare, container: CKContainer, allowedSharingOptions: CKAllowedSharingOptions) -> CKShareTransferRepresentation&lt;Item>.ExportedShare

Allows the user to view or make modifications to the share settings.

static func prepareShare(container: CKContainer, allowedSharingOptions: CKAllowedSharingOptions, preparationHandler: () async throws -> CKShare) -> CKShareTransferRepresentation&lt;Item>.ExportedShare

Creates a share when the system calls the specified handler.

## Relationships

### Conforms To

- Sendable
- Transferable

