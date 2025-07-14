

- CloudKit
- CKFetchRecordsOperation
-  init(recordIDs:) 

Initializer

# init(recordIDs:)

Creates a fetch operation for retrieving the records with the specified IDs.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
convenience init(recordIDs: [CKRecord.ID])
```

## Parameters 

`recordIDs`  

An array of CKRecord.ID objects that represents the records you want to retrieve. If you provide an empty array, you must set the recordIDs property before you execute the operation.

## Discussion

A fetch operation retrieves all of a record’s fields, including any assets that those fields reference. If you want to minimize the amount of data that the operation returns, configure the desiredKeys property with only the keys that contain the values that you have an interest in.

After initializing the operation, you must associate at least one progress handler with the operation (excluding the completion handler) to process the results.

## See Also

### Creating a Record Fetch Operation

init()

Creates an empty fetch operation.

