

- CloudKit
- CKFetchRecordZoneChangesOperation
- CKFetchRecordZoneChangesOperation.ZoneConfiguration
-  resultsLimit 

Instance Property

# resultsLimit

The maximum number of records that CloudKit retrieves when fetching zone changes.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var resultsLimit: Int { get set }
```

## See Also

### Accessing a Zone Change Configuration

var previousServerChangeToken: CKServerChangeToken?

The server change token.

var desiredKeys: [CKRecord.FieldKey]?

An array of the record keys to retrieve.

