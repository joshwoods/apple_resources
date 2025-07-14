

- CloudKit
- CKDatabase
-  save(\_:completionHandler:) 

Instance Method

# save(\_:completionHandler:)

Saves a specific record zone.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func save(
    _ zone: CKRecordZone,
    completionHandler: @escaping (CKRecordZone?, (any Error)?) -> Void
)
```

``` source
func save(_ zone: CKRecordZone) async throws -> CKRecordZone
```

## Parameters 

`zone`  

The record zone to save.

`completionHandler`  

The closure to execute after CloudKit saves the record.

## Discussion

The completion handler takes the following parameters:

- The saved record zone (as it appears on the server), or `nil` if there’s an error.

- An error if a problem occurs, or `nil` if CloudKit successfully saves the record zone.

For information on a more convenient way to save record zones, see modifyRecordZones(saving:deleting:).

## See Also

### Modifying Record Zones

func modifyRecordZones(saving: [CKRecordZone], deleting: [CKRecordZone.ID]) async throws -> (saveResults: [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], deleteResults: [CKRecordZone.ID : Result&lt;Void, any Error>])

Modifies the specified record zones and returns the results to an awaiting caller.

func modifyRecordZones(saving: [CKRecordZone], deleting: [CKRecordZone.ID], completionHandler: (Result&lt;(saveResults: [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], deleteResults: [CKRecordZone.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified record zones and delivers the results to a completion handler.

func delete(withRecordZoneID: CKRecordZone.ID, completionHandler: (CKRecordZone.ID?, (any Error)?) -> Void)

Deletes a specific record zone.

