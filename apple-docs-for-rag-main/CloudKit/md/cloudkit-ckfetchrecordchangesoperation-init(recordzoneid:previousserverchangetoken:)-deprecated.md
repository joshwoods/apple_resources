

- CloudKit
- CKFetchRecordChangesOperation
-  init(recordZoneID:previousServerChangeToken:) Deprecated

Initializer

# init(recordZoneID:previousServerChangeToken:)

Creates an operation for fetching changes in the specified record zone.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
convenience init(
    recordZoneID: CKRecordZone.ID,
    previousServerChangeToken: CKServerChangeToken?
)
```

## Parameters 

`recordZoneID`  

The zone that contains the records you want to fetch. The zone can be a custom zone. The system doesn’t support syncing the default zone.

`previousServerChangeToken`  

The change token from a previous fetch operation. This is the token that the system passes to your fetchRecordChangesCompletionBlock handler during a previous fetch operation. Use this token to limit the returned data to only those changes that occur after that fetch request. If you specify `nil` for this parameter, the operation object fetches all records and their contents.

## Return Value

An initialized operation object.

## Discussion

When initializing the operation object, use the token from a previous fetch request if you have one. You can archive tokens and write them to disk for later use.

The returned operation object retrieves all changed fields of the record, including any assets in those fields. If you want to minimize the amount of data that returns even further, configure the desiredKeys property with the subset of keys that have values you want to fetch.

After initializing the operation, associate at least one progress block with the operation object (excluding the completion block) to process the results.

## See Also

### Creating the Fetch Record Changes Operation

init()

Creates an empty fetch record changes operation.

Deprecated

