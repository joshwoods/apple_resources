

- CloudKit
- CKModifyRecordsOperation
-  clientChangeTokenData 

Instance Property

# clientChangeTokenData

A token that tracks local changes to records.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var clientChangeTokenData: Data? { get set }
```

## Discussion

The default value is `nil`.

When you modify records from a fetch operation, specify a token using this property to indicate which version of the record you most recently modified. Compare the token you supply to the token in the next record fetch to confirm the server successfully receives the device’s most recent modify request.

If you intend to change the value of this property, do so before you execute the operation or submit the operation to a queue.

## See Also

### Configuring the Modify Record Operation

var recordsToSave: [CKRecord]?

The records to save to the database.

var recordIDsToDelete: [CKRecord.ID]?

The IDs of the records to delete permanently from the database.

var isAtomic: Bool

A Boolean value that indicates whether the entire operation fails when CloudKit can’t update one or more records in a record zone.

var savePolicy: CKModifyRecordsOperation.RecordSavePolicy

The policy to use when saving changes to records.

enum RecordSavePolicy

Constants that indicate which policy to apply when saving records.

