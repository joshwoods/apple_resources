

- CloudKit
- CKDatabase
-  recordZones(for:) 

Instance Method

# recordZones(for:)

Fetches the specified record zones and returns them to an awaiting caller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func recordZones(for ids: [CKRecordZone.ID]) async throws -> [CKRecordZone.ID : Result]
```

## Parameters 

`ids`  

The identifiers of the record zones to fetch.

## Return Value

A dictionary that contains the fetched record zones. The dictionary uses the specified record zone identifiers as its keys. The value of each key is a Result that contains either the corresponding fetched record zone, or an error that describes why CloudKit can’t provide that record zone.

## Discussion

This method throws an error if the request fails, such as when the network is unavailable or the device doesn’t have an active iCloud account; otherwise, the returned dictionary includes any individual record zone errors.

For information on a more configurable way to fetch specific record zones, see CKFetchRecordZonesOperation.

## See Also

### Fetching Record Zones

func fetch(withRecordZoneIDs: [CKRecordZone.ID], completionHandler: (Result&lt;[CKRecordZone.ID : Result&lt;CKRecordZone, any Error>], any Error>) -> Void)

Fetches the specified record zones and delivers them to a completion handler.

func fetchAllRecordZones(completionHandler: ([CKRecordZone]?, (any Error)?) -> Void)

Fetches all record zones from the current database.

func fetch(withRecordZoneID: CKRecordZone.ID, completionHandler: (CKRecordZone?, (any Error)?) -> Void)

Fetches a specific record zone.

