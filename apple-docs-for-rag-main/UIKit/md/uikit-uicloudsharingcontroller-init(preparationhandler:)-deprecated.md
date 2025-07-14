

- UIKit
- UICloudSharingController
-  init(preparationHandler:) Deprecated

Initializer

# init(preparationHandler:)

Initializes the CloudKit sharing controller with a preparation handler intending to save a new share record.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
init(preparationHandler: @escaping (UICloudSharingController, @escaping (CKShare?, CKContainer?, (any Error)?) -> Void) -> Void)
```

## Parameters 

`preparationHandler`  

The block invoked by UICloudSharingController when it is time for your application to save a newly created CKShare record.

## Discussion

Use the init(preparationHandler:) initializer method to create a new UICloudSharingController instance when the user who owns a CKRecord wants to share the record with other people. To determine if the record is shared, check its share property. If the property value is `nil`, the record is not shared, and this method is the one to use.

Important

You must initialize the controller with the correct initializer method. Do not use init(preparationHandler:) if the CKRecord is already shared. Likewise, do not use init(share:container:) if the CKRecord is not shared. Using the wrong initializer leads to errors when saving the record.

The `preparationHandler:` provided to the initializer method is responsible for saving the new CKShare record. The handler has two parameters:

- A reference to the UICloudSharingController instance that called the preparation handler

- A reference to a completion block

After you save the new CKShare record and its root record (the CKRecord representing the data to share) in the preparation handler, you call the completion block. Calling the completion block tells the UICloudSharingController instance to continue with the invitation workflow.

For more information and sample code, see Inviting participants to a new share.

## See Also

### Creating the cloud sharing controller

init(share: CKShare, container: CKContainer)

Initializes the CloudKit sharing view controller with a CloudKit share record and container to manage participants and restrictions.

