

- CloudKit
- CKFetchRecordZoneChangesOperation
-  fetchAllChanges 

Instance Property

# fetchAllChanges

A Boolean value that indicates whether to send repeated requests to the server.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var fetchAllChanges: Bool { get set }
```

## Discussion

If true, the operation sends repeat requests to the server until it fetches all changes. CloudKit executes the handler you set on the recordZoneFetchCompletionBlock property with a change token after each request.

The default value is true.

## See Also

### Configuring the Zone Change Operation

var configurationsByRecordZoneID: [CKRecordZone.ID : CKFetchRecordZoneChangesOperation.ZoneConfiguration]?

A dictionary of configurations for fetching change operations by zone identifier.

class ZoneConfiguration

A configuration object that describes the information to fetch from a record zone.

var recordZoneIDs: [CKRecordZone.ID]?

The IDs of the record zones that contain the records to fetch.

