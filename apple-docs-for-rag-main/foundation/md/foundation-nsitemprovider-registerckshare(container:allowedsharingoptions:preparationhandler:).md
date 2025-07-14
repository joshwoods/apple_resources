

- Foundation
- NSItemProvider
-  registerCKShare(container:allowedSharingOptions:preparationHandler:) 

Instance Method

# registerCKShare(container:allowedSharingOptions:preparationHandler:)

Creates and registers a new collaboration object using a collection of records to share.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func registerCKShare(
    container: CKContainer,
    allowedSharingOptions: CKAllowedSharingOptions = CKAllowedSharingOptions.standard,
    preparationHandler: @escaping () async throws -> CKShare
)
```

## Parameters 

`container`  

A CKContainer the system uses to coordinate all the interactions between your app and the server.

`allowedSharingOptions`  

The CKAllowedSharingOptions. The standard option is the default.

`preparationHandler`  

The handler the system calls in your app to create a new CKShare.

## Discussion

Use this method to share a collection of CKRecord objects that don’t have an existing CKShare assignment. When the system calls the `preparationHandler`, your app creates a new `CKShare` with the appropriate root `CKRecord` or CKRecordZone.ID.

After the server successfully saves the share, invoke the CKSharePreparationCompletionHandler with either the resulting `CKShare`, or an `NSError` if the save fails.

When the system invokes the share sheet with a `CKShare` that you register with this method, it prompts the user to start sharing.

## See Also

### Registering CloudKit shares

func registerCloudKitShare(CKShare, container: CKContainer)

Registers a CloudKit share for the user to modify.

func registerCloudKitShare(preparationHandler: ((CKShare?, CKContainer?, (any Error)?) -> Void) -> Void)

Registers a handler that prepares a new CloudKit share.

func registerCKShare(CKShare, container: CKContainer, allowedSharingOptions: CKAllowedSharingOptions)

Registers an existing collaboration object on a server.

