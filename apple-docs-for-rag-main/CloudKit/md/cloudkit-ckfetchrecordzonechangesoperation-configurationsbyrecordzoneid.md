

- CloudKit
- CKFetchRecordZoneChangesOperation
-  configurationsByRecordZoneID 

Instance Property

# configurationsByRecordZoneID

A dictionary of configurations for fetching change operations by zone identifier.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var configurationsByRecordZoneID: [CKRecordZone.ID : CKFetchRecordZoneChangesOperation.ZoneConfiguration]? { get set }
```

## See Also

### Configuring the Zone Change Operation

class ZoneConfiguration

A configuration object that describes the information to fetch from a record zone.

var fetchAllChanges: Bool

A Boolean value that indicates whether to send repeated requests to the server.

var recordZoneIDs: [CKRecordZone.ID]?

The IDs of the record zones that contain the records to fetch.

