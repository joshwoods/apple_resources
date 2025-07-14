

- CloudKit
- CKModifyRecordZonesOperation
-  init(recordZonesToSave:recordZoneIDsToDelete:) 

Initializer

# init(recordZonesToSave:recordZoneIDsToDelete:)

Creates an operation for modifying the specified record zones.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
convenience init(
    recordZonesToSave: [CKRecordZone]? = nil,
    recordZoneIDsToDelete: [CKRecordZone.ID]? = nil
)
```

## Parameters 

`recordZonesToSave`  

The record zones to save. You can specify `nil` for this parameter.

`recordZoneIDsToDelete`  

The IDs of the record zones to delete. You can specify `nil` for this parameter.

## Discussion

The record zones you intend to save or delete must all reside in the same database, which you specify when you configure the operation. If you delete a record zone, CloudKit deletes any records it contains.

## See Also

### Creating a Modify Zones Operation

init()

Creates an empty modify record zones operation.

