

- Foundation
- NSItemProvider
-  registerCKShare(\_:container:allowedSharingOptions:) 

Instance Method

# registerCKShare(\_:container:allowedSharingOptions:)

Registers an existing collaboration object on a server.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func registerCKShare(
    _ share: CKShare,
    container: CKContainer,
    allowedSharingOptions: CKAllowedSharingOptions = CKAllowedSharingOptions.standard
)
```

## Parameters 

`share`  

An existing CKShare on the server.

`container`  

A CKContainer the system uses to coordinate all the interactions between your app and the server.

`allowedSharingOptions`  

The CKAllowedSharingOptions. The standard option is the default.

## Discussion

Use this method when a CKShare currently exists on the server. When the system invokes the share sheet with a `CKShare` that you register with this method, it allows the owner to make modifications to the share settings, and allows a participant to view the share settings.

## See Also

### Registering CloudKit shares

func registerCloudKitShare(CKShare, container: CKContainer)

Registers a CloudKit share for the user to modify.

func registerCloudKitShare(preparationHandler: ((CKShare?, CKContainer?, (any Error)?) -> Void) -> Void)

Registers a handler that prepares a new CloudKit share.

func registerCKShare(container: CKContainer, allowedSharingOptions: CKAllowedSharingOptions, preparationHandler: () async throws -> CKShare)

Creates and registers a new collaboration object using a collection of records to share.

