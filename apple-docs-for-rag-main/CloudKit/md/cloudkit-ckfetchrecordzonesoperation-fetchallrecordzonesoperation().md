

- CloudKit
- CKFetchRecordZonesOperation
-  fetchAllRecordZonesOperation() 

Type Method

# fetchAllRecordZonesOperation()

Returns an operation for fetching all record zones in the current database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class func fetchAllRecordZonesOperation() -> Self
```

## Discussion

Assign a value to the fetchRecordZonesCompletionBlock property of the operation that this method returns so that you can process the results.

