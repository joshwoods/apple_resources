

- CloudKit
- CKDatabase
-  modifyRecordZones(saving:deleting:completionHandler:) 

Instance Method

# modifyRecordZones(saving:deleting:completionHandler:)

Modifies the specified record zones and delivers the results to a completion handler.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
@preconcurrency
func modifyRecordZones(
    saving recordZonesToSave: [CKRecordZone],
    deleting recordZoneIDsToDelete: [CKRecordZone.ID],
    completionHandler: @escaping (Result], deleteResults: [CKRecordZone.ID : Result]), any Error>) -> Void
)
```

## Parameters 

`recordZonesToSave`  

The record zones to save.

`recordZoneIDsToDelete`  

The identifiers of the record zones to permanently delete.

`completionHandler`  

The closure to execute after CloudKit processes the changes.

## Discussion

Warning

Deleting a record zone is a permanent action that deletes every record in that zone. You can’t restore a deleted record zone.

The completion handler takes a single Result parameter that contains either a tuple, or an error if the request fails. For example, when the network is unavailable or the device doesn’t have an active iCloud account.

When present, the tuple contains the following named elements:

`saveResults`  
A dictionary of saved record zones. The dictionary uses the identifiers of the record zones you specify in `recordsZonesToSave` as its keys. The value of each key is a Result that contains either the corresponding modified record zone (as it appears on the server), or an error that describes why CloudKit can’t modify that record.

`deleteResults`  
A dictionary of deleted record zones. The dictionary uses the identifiers you specify in `recordZoneIDsToDelete` as its keys. The value of each key is a Result that contains either Void to indicate a successful deletion, or an error that describes why CloudKit can’t delete that record zone.

For information on a more configurable way to modify record zones, see CKModifyRecordZonesOperation.

## See Also

### Modifying Record Zones

func modifyRecordZones(saving: [CKRecordZone], deleting: [CKRecordZone.ID]) async throws -> (saveResults: [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], deleteResults: [CKRecordZone.ID : Result&lt;Void, any Error>])

Modifies the specified record zones and returns the results to an awaiting caller.

func save(CKRecordZone, completionHandler: (CKRecordZone?, (any Error)?) -> Void)

Saves a specific record zone.

func delete(withRecordZoneID: CKRecordZone.ID, completionHandler: (CKRecordZone.ID?, (any Error)?) -> Void)

Deletes a specific record zone.

