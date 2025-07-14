

- CloudKit
- CKFetchRecordChangesOperation
-  recordZoneID Deprecated

Instance Property

# recordZoneID

The ID of the record zone with the records you want to fetch.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
@NSCopying
var recordZoneID: CKRecordZone.ID? { get set }
```

## Discussion

Typically, you set the value of this property when you initialize the operation object. If you intend to change the record zone, update the value before executing the operation or submitting it to a queue.

## See Also

### Configuring the Fetch Record Changes Operation

var previousServerChangeToken: CKServerChangeToken?

The token that identifies the starting point for retrieving changes.

Deprecated

var desiredKeys: [String]?

The fields to fetch for the requested records.

Deprecated

var resultsLimit: Int

The maximum number of changed records to report with this operation object.

Deprecated

var moreComing: Bool

A Boolean value that indicates whether more results are available.

Deprecated

