

- CloudKit
- CKFetchRecordChangesOperation
-  resultsLimit Deprecated

Instance Property

# resultsLimit

The maximum number of changed records to report with this operation object.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var resultsLimit: Int { get set }
```

## Discussion

Use this property to limit the number of results in situations where you expect the number of changed records to be large. The default value is 0, which causes the server to return an appropriate number of results using dynamic conditions.

When the number of returned results exceeds the results limit, the operation object sets the moreComing property to true before executing the block in the fetchRecordChangesCompletionBlock property. In your block, check the value of that property, and if it’s true, create a new CKFetchRecordChangesOperation object to fetch more results.

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

var moreComing: Bool

A Boolean value that indicates whether more results are available.

Deprecated

