

- CloudKit
- CKDatabase
-  fetchAllRecordZones(completionHandler:) 

Instance Method

# fetchAllRecordZones(completionHandler:)

Fetches all record zones from the current database.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func fetchAllRecordZones(completionHandler: @escaping ([CKRecordZone]?, (any Error)?) -> Void)
```

``` source
func allRecordZones() async throws -> [CKRecordZone]
```

## Parameters 

`completionHandler`  

The closure to execute with the fetch results.

## Discussion

The completion handler takes the following parameters:

- An array of fetched record zones, or `nil` if there’s an error. When present, the array contains at least one record zone, the default zone.

- An error if a problem occurs, or `nil` if CloudKit successfully fetches all record zones.

## See Also

### Fetching Record Zones

func recordZones(for: [CKRecordZone.ID]) async throws -> [CKRecordZone.ID : Result&lt;CKRecordZone, any Error>]

Fetches the specified record zones and returns them to an awaiting caller.

func fetch(withRecordZoneIDs: [CKRecordZone.ID], completionHandler: (Result&lt;[CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], any Error>) -> Void)

Fetches the specified record zones and delivers them to a completion handler.

func fetch(withRecordZoneID: CKRecordZone.ID, completionHandler: (CKRecordZone?, (any Error)?) -> Void)

Fetches a specific record zone.

