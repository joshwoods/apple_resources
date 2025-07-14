

- CloudKit
- CKModifyRecordZonesOperation
-  recordZoneIDsToDelete 

Instance Property

# recordZoneIDsToDelete

The IDs of the record zones to delete permanently from the database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var recordZoneIDsToDelete: [CKRecordZone.ID]? { get set }
```

## Discussion

The initial value of the property is the array of zone IDs that you provide to the initWithRecordZonesToSave:recordZoneIDsToDelete: method. You can modify this array as necessary before you execute the operation. The record zones must all target the same database. You can specify `nil`, or an empty array, for this property.

If you intend to change the value of this property, do so before you execute the operation or submit the operation to a queue.

## See Also

### Configuring the Modify Zones Operation

var recordZonesToSave: [CKRecordZone]?

The record zones to save to the database.

