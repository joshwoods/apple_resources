

- CloudKit
- CKShareTransferRepresentation
- CKShareTransferRepresentation.ExportedShare
-  prepareShare(container:allowedSharingOptions:preparationHandler:) 

Type Method

# prepareShare(container:allowedSharingOptions:preparationHandler:)

Creates a share when the system calls the specified handler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS

``` source
static func prepareShare(
    container: CKContainer,
    allowedSharingOptions: CKAllowedSharingOptions = CKAllowedSharingOptions.standard,
    preparationHandler: @escaping () async throws -> CKShare
) -> CKShareTransferRepresentation.ExportedShare
```

## Parameters 

`container`  

The CKContainer for the share.

`allowedSharingOptions`  

The CKAllowedSharingOptions. The standard option is the default.

`preparationHandler`  

The handler the system calls in your app to create a new CKShare.

## Return Value

The CKShareTransferRepresentation.ExportedShare with the new `CKShare`.

## Discussion

Use this method when you want to share a collection of CKRecord objects, but don’t currently have a CKShare.

When the system calls the `preparationHandler`, create a new `CKShare` with the appropriate root `CKRecord` or CKRecordZone.ID.

After saving the share and all records to the server, return the resulting `CKShare` or throw an error if saving fails. When your app invokes the share sheet with a `CKShare`, the system prompts the user to start sharing.

## See Also

### Preparing an exported share

static func existing(CKShare, container: CKContainer, allowedSharingOptions: CKAllowedSharingOptions) -> CKShareTransferRepresentation&lt;Item>.ExportedShare

Allows the user to view or make modifications to the share settings.

