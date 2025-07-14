

- CloudKit
- CKQueryNotification
-  recordID 

Instance Property

# recordID

The ID of the record that CloudKit creates, updates, or deletes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var recordID: CKRecord.ID? { get }
```

## Discussion

Use this value to fetch the record.

## See Also

### Getting the Record Information

var recordFields: [String : Any]?

A dictionary of fields that have changes.

