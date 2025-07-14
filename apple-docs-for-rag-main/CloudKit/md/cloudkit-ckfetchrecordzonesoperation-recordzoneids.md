

- CloudKit
- CKFetchRecordZonesOperation
-  recordZoneIDs 

Instance Property

# recordZoneIDs

The IDs of the record zones to retrieve.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var recordZoneIDs: [CKRecordZone.ID]? { get set }
```

## Discussion

Use this property to view or change the IDs of the record zones you want to retrieve. If you intend to change the value of this property, do so before you execute the operation or submit the operation to a queue.

If you use the operation that fetchAllRecordZonesOperation() returns, CloudKit ignores the contents of this property and sets its value to `nil`.

