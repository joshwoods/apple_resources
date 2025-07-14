

- CloudKit
- CKFetchRecordZonesOperation
-  init() 

Initializer

# init()

Creates an empty fetch zones operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
init()
```

## Discussion

You must set the recordZoneIDs property before you execute the operation.

After creating the operation, assign a value to the fetchRecordZonesCompletionBlock property so you can process the results.

## See Also

### Initializing the Zone Fetch Operation

convenience init(recordZoneIDs: [CKRecordZone.ID])

Creates an operation for fetching the specified record zones.

