

- CloudKit
- CKShareTransferRepresentation
- CKShareTransferRepresentation.ExportedShare
-  existing(\_:container:allowedSharingOptions:) 

Type Method

# existing(\_:container:allowedSharingOptions:)

Allows the user to view or make modifications to the share settings.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS

``` source
static func existing(
    _ share: CKShare,
    container: CKContainer,
    allowedSharingOptions: CKAllowedSharingOptions = CKAllowedSharingOptions.standard
) -> CKShareTransferRepresentation.ExportedShare
```

## Parameters 

`share`  

The existing `CKShare` object.

`container`  

The CKContainer for the share.

`allowedSharingOptions`  

The CKAllowedSharingOptions. The standard option is the default.

## Return Value

The CKShareTransferRepresentation.ExportedShare with updated share settings.

## Discussion

Use this method when you have a share that’s already saved to the server.

When the system invokes the share sheet with a CKShare registered with this method, the system allows the owner to make modifications to the share settings, or allows a participant to view the share settings.

## See Also

### Preparing an exported share

static func prepareShare(container: CKContainer, allowedSharingOptions: CKAllowedSharingOptions, preparationHandler: () async throws -> CKShare) -> CKShareTransferRepresentation&lt;Item>.ExportedShare

Creates a share when the system calls the specified handler.

