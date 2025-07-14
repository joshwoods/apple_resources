

- CloudKit
- CKError
-  serverRecord 

Instance Property

# serverRecord

The server’s version of the record.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+

``` source
var serverRecord: CKRecord? { get }
```

## Discussion

This property’s value is available only when the error’s `code` is serverRecordChanged, which indicates the server’s record is newer than the version you try to save. Use this property’s value, along with those of ancestorRecord and clientRecord, to resolve the conflict.

The error’s `userInfo` dictionary contains the same value as this property. You can access it using the CKRecordChangedErrorServerRecordKey key.

## See Also

### Getting Conflicted Records

var ancestorRecord: CKRecord?

The original version of the record.

var clientRecord: CKRecord?

The local version of the record that includes any changes.

