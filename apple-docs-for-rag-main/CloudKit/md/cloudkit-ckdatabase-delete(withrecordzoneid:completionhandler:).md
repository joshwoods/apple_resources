

- CloudKit
- CKDatabase
-  delete(withRecordZoneID:completionHandler:) 

Instance Method

# delete(withRecordZoneID:completionHandler:)

Deletes a specific record zone.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func delete(
    withRecordZoneID zoneID: CKRecordZone.ID,
    completionHandler: @escaping (CKRecordZone.ID?, (any Error)?) -> Void
)
```

``` source
func deleteRecordZone(withID zoneID: CKRecordZone.ID) async throws -> CKRecordZone.ID
```

## Parameters 

`zoneID`  

The identifier of the record zone to delete.

`completionHandler`  

The closure to execute after CloudKit deletes the record zone.

## Discussion

Warning

Deleting a record zone is a permanent action that deletes every record in that zone. You can’t restore a deleted record zone.

The completion handler takes the following parameters:

- The identifier of the deleted record zone, or `nil` if there’s an error.

- An error if a problem occurs, or `nil` if CloudKit successfully deletes the record zone.

For information on a more convenient way to delete record zones, see modifyRecordZones(saving:deleting:).

## See Also

### Modifying Record Zones

func modifyRecordZones(saving: [CKRecordZone], deleting: [CKRecordZone.ID]) async throws -> (saveResults: [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], deleteResults: [CKRecordZone.ID : Result&lt;Void, any Error>])

Modifies the specified record zones and returns the results to an awaiting caller.

func modifyRecordZones(saving: [CKRecordZone], deleting: [CKRecordZone.ID], completionHandler: (Result&lt;(saveResults: [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], deleteResults: [CKRecordZone.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified record zones and delivers the results to a completion handler.

func save(CKRecordZone, completionHandler: (CKRecordZone?, (any Error)?) -> Void)

Saves a specific record zone.

