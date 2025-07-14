

- CloudKit
- CKFetchRecordZoneChangesOperation
-  recordZoneIDs 

Instance Property

# recordZoneIDs

The IDs of the record zones that contain the records to fetch.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var recordZoneIDs: [CKRecordZone.ID]? { get set }
```

## Discussion

Typically, you set the value of this property when you create the operation. If you intend to change the record zone IDs, update the value before you execute the operation or submit it to a queue.

## See Also

### Configuring the Zone Change Operation

var configurationsByRecordZoneID: [CKRecordZone.ID : CKFetchRecordZoneChangesOperation.ZoneConfiguration]?

A dictionary of configurations for fetching change operations by zone identifier.

class ZoneConfiguration

A configuration object that describes the information to fetch from a record zone.

var fetchAllChanges: Bool

A Boolean value that indicates whether to send repeated requests to the server.

