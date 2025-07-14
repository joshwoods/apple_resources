

- CloudKit
- CKFetchRecordsOperation
-  fetchCurrentUserRecordOperation() 

Type Method

# fetchCurrentUserRecordOperation()

Returns a fetch operation for retrieving the current user record.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class func fetchCurrentUserRecordOperation() -> Self
```

## Discussion

The returned operation object searches for the single record that corresponds to the current user record. You must associate at least one progress handler with the operation object (excluding the completion handler) to process the results.

