

- CloudKit
- CKFetchRecordChangesOperation
-  moreComing Deprecated

Instance Property

# moreComing

A Boolean value that indicates whether more results are available.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var moreComing: Bool { get }
```

## Discussion

If the server is unable to deliver all of the changed results with this operation object, it sets this property to true before executing the block in the fetchRecordChangesCompletionBlock property. To fetch the remaining changes, create a new CKFetchRecordChangesOperation object using the change token that the server returns.

## See Also

### Configuring the Fetch Record Changes Operation

var recordZoneID: CKRecordZone.ID?

The ID of the record zone with the records you want to fetch.

Deprecated

var previousServerChangeToken: CKServerChangeToken?

The token that identifies the starting point for retrieving changes.

Deprecated

var desiredKeys: [String]?

The fields to fetch for the requested records.

Deprecated

var resultsLimit: Int

The maximum number of changed records to report with this operation object.

Deprecated

