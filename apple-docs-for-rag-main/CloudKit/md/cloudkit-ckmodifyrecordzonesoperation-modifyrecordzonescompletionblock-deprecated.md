

- CloudKit
- CKModifyRecordZonesOperation
-  modifyRecordZonesCompletionBlock Deprecated

Instance Property

# modifyRecordZonesCompletionBlock

The closure to execute after CloudKit modifies all of the record zones.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var modifyRecordZonesCompletionBlock: (([CKRecordZone]?, [CKRecordZone.ID]?, (any Error)?) -> Void)? { get set }
```

Deprecated

Use modifyRecordZonesResultBlock instead

## Discussion

This property is a closure that returns no value and has the following parameters:

- The record zones that CloudKit saves.

- The IDs of the record zones that CloudKit deletes.

- If CloudKit can’t modify any of the record zones, this parameter provides information about the failure; otherwise, it’s `nil`.

The closure executes once, and represents your only opportunity to process the results.

The closure reports an error of type CKError.Code.partialFailure when it modifies only some of the record zones successfully. The userInfo dictionary of the error contains a CKPartialErrorsByItemIDKey key that has a dictionary as its value. The keys of the dictionary are the IDs of the record zones that the operation can’t modify, and the corresponding values are errors that contain information about the failures.

If you intend to use this closure to process the results, set it before you execute the operation or submit the operation to a queue.

