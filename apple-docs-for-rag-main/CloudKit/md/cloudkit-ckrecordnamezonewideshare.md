

- CloudKit
-  CKRecordNameZoneWideShare 

Global Variable

# CKRecordNameZoneWideShare

The name of a share record that manages a shared record zone.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let CKRecordNameZoneWideShare: String
```

## Discussion

When you create an instance of CKShare for sharing a record zone, CloudKit automatically assigns this constant as the recordName element of the share record’s recordID. After you save the share record to iCloud, you can fetch it by reconstructing the record ID using this constant, as the following example shows:

```
func fetchShare(forZone zone: CKRecordZone,
                completion: @escaping (Result) -> Void) {
    let database = CKContainer.default().privateCloudDatabase

    // Use the 'CKRecordNameZoneWideShare' constant to create the record ID.
    let recordID = CKRecord.ID(recordName: CKRecordNameZoneWideShare,
                               zoneID: zone.zoneID)

    // Fetch the share record from the specified record zone.
    database.fetch(withRecordID: recordID) { share, error in
        if let error = error {
            // If the fetch fails, inform the caller.
            completion(.failure(error))
        } else if let share = share as? CKShare {
            // Otherwise, pass the fetched share record to the
            // completion handler.
            completion(.success(share))
        } else {
            fatalError("Unable to fetch record with ID: \(recordID)")
        }
    }
}
```

## See Also

### Creating a Record ID

convenience init(recordName: String)

Creates a new record ID with the specified name in the default zone.

convenience init(recordName: String, zoneID: CKRecordZone.ID)

Creates a new record ID with the specified name and zone information.

