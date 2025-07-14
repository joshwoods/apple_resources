

- CloudKit
- CKFetchRecordZoneChangesOperation
- CKFetchRecordZoneChangesOperation.ZoneConfiguration
-  previousServerChangeToken 

Instance Property

# previousServerChangeToken

The server change token.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@NSCopying
var previousServerChangeToken: CKServerChangeToken? { get set }
```

## See Also

### Accessing a Zone Change Configuration

var resultsLimit: Int

The maximum number of records that CloudKit retrieves when fetching zone changes.

var desiredKeys: [CKRecord.FieldKey]?

An array of the record keys to retrieve.

