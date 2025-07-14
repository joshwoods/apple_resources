

- CloudKit
- CKFetchRecordChangesOperation
-  desiredKeys Deprecated

Instance Property

# desiredKeys

The fields to fetch for the requested records.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var desiredKeys: [String]? { get set }
```

## Discussion

Use this property to limit the amount of data that the system retrieves for each record during the fetch operation. This property contains an array of strings, each of which contains the name of a field from the target records. When you retrieve a record, the returned records only include fields with names that match one of the keys in this property. The default value is `nil`, which causes the system to fetch all keys of the record.

Because the records you fetch can be of different types, configure the array to include the merged set of all field names for the requested records and at least one field name from each record type.

If you intend to specify the desired set of keys, set the value of this property before executing the operation or submitting it to a queue.

## See Also

### Configuring the Fetch Record Changes Operation

var recordZoneID: CKRecordZone.ID?

The ID of the record zone with the records you want to fetch.

Deprecated

var previousServerChangeToken: CKServerChangeToken?

The token that identifies the starting point for retrieving changes.

Deprecated

var resultsLimit: Int

The maximum number of changed records to report with this operation object.

Deprecated

var moreComing: Bool

A Boolean value that indicates whether more results are available.

Deprecated

