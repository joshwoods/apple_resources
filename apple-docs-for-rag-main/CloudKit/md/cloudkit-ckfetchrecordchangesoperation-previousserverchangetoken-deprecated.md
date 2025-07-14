

- CloudKit
- CKFetchRecordChangesOperation
-  previousServerChangeToken Deprecated

Instance Property

# previousServerChangeToken

The token that identifies the starting point for retrieving changes.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
@NSCopying
var previousServerChangeToken: CKServerChangeToken? { get set }
```

## Discussion

Each fetch request returns a unique token in addition to any changes. The token passes as a parameter to your fetchRecordChangesCompletionBlock handler. During a subsequent fetch request, providing the previous token causes the server to return only the changes that occur after the previous fetch request. Tokens are opaque data objects that you can write to disk safely and reuse later.

Typically, you set the value of this property when you initialize the operation object. If you intend to change the record zone, update the value of the property before executing the operation or submitting it to a queue.

## See Also

### Configuring the Fetch Record Changes Operation

var recordZoneID: CKRecordZone.ID?

The ID of the record zone with the records you want to fetch.

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

