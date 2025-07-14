

- UIKit
- UICloudSharingController
-  init(share:container:) 

Initializer

# init(share:container:)

Initializes the CloudKit sharing view controller with a CloudKit share record and container to manage participants and restrictions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    share: CKShare,
    container: CKContainer
)
```

## Parameters 

`share`  

An instance of CKShare that was previously saved.

`container`  

An instance of CKContainer that contains the record that is shared.

## Discussion

Use the init(share:container:) initializer method to create the UICloudSharingController instance when the user who owns the CKShare record wants to manage the participants and restrictions associated with the share. (For more information, see Adding and removing participants from an existing share.) You also use this initializer method when users are participants who want to remove themselves from a share. (For more information, see Viewing participants and leaving a share.)

Important

You must initialize the controller with the correct initializer method. Do not use init(preparationHandler:) if the CKRecord is already shared. Likewise, do not use init(share:container:) if the CKRecord is not shared. Using the wrong initializer leads to errors when saving the record.

init(share:container:) requires a reference to the CKShare instance associated with the CKRecord instance that represents the shared data. To retrieve the CKShare instance, get the share property value (a CKRecord.Reference instance) from the CKRecord instance. Then pass the recordID from the CKRecord.Reference instance to the fetch(withRecordID:completionHandler:) method on a CKDatabase instance, as shown in the following code.

```
CKRecord *record = [self record];
CKReference *shareReference = [record share];
if (shareReference == nil) {
  return;
}
CKContainer *container = [CKContainer defaultContainer];
[[container privateCloudDatabase] fetchRecordWithID:[shareReference recordID] completionHandler:^(CKRecord * _Nullable record, NSError * _Nullable error) {

  if (record == nil) {
    NSLog(@"%@", [error localizedDescription]);
  } else if ([record isKindOfClass:[CKShare class]]) {
    CKShare *shareRecord = (CKShare *)record;
    NSLog(@"%@", [shareRecord URL]);
  }

}];
```

## See Also

### Creating the cloud sharing controller

init(preparationHandler: (UICloudSharingController, (CKShare?, CKContainer?, (any Error)?) -> Void) -> Void)

Initializes the CloudKit sharing controller with a preparation handler intending to save a new share record.

Deprecated

