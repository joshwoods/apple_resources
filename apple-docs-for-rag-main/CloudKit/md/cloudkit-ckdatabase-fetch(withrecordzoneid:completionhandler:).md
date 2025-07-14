

- CloudKit
- CKDatabase
-  fetch(withRecordZoneID:completionHandler:) 

Instance Method

# fetch(withRecordZoneID:completionHandler:)

Fetches a specific record zone.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func fetch(
    withRecordZoneID zoneID: CKRecordZone.ID,
    completionHandler: @escaping (CKRecordZone?, (any Error)?) -> Void
)
```

``` source
func recordZone(for zoneID: CKRecordZone.ID) async throws -> CKRecordZone
```

## Parameters 

`zoneID`  

The identifier of the record zone to fetch.

`completionHandler`  

The closure to execute with the fetch results.

## Discussion

The completion handler takes the following parameters:

- The fetched record zone, or `nil` if there’s an error.

- An error if a problem occurs, or `nil` if CloudKit successfully fetches the specified record zone.

For information on a more convenient way to fetch specific record zones, see recordZones(for:) in Swift or CKFetchRecordZonesOperation in Objective-C.

## See Also

### Fetching Record Zones

func recordZones(for: [CKRecordZone.ID]) async throws -> [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>]

Fetches the specified record zones and returns them to an awaiting caller.

func fetch(withRecordZoneIDs: [CKRecordZone.ID], completionHandler: (Result&lt;[CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], any Error>) -> Void)

Fetches the specified record zones and delivers them to a completion handler.

func fetchAllRecordZones(completionHandler: ([CKRecordZone]?, (any Error)?) -> Void)

Fetches all record zones from the current database.

