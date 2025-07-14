

- CloudKit
- CKFetchRecordZoneChangesOperation
- CKFetchRecordZoneChangesOperation.ZoneConfiguration
-  desiredKeys 

Instance Property

# desiredKeys

An array of the record keys to retrieve.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOSwatchOS 5.0+Swift 4.2+

``` source
var desiredKeys: [CKRecord.FieldKey]? { get set }
```

## See Also

### Accessing a Zone Change Configuration

var previousServerChangeToken: CKServerChangeToken?

The server change token.

var resultsLimit: Int

The maximum number of records that CloudKit retrieves when fetching zone changes.

