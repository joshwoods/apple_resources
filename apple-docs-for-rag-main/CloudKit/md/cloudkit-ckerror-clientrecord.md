

- CloudKit
- CKError
-  clientRecord 

Instance Property

# clientRecord

The local version of the record that includes any changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+

``` source
var clientRecord: CKRecord? { get }
```

## Discussion

This property’s value is available only when the error’s `code` is serverRecordChanged, which indicates the server’s record is newer than the version you try to save. Use this property’s value, along with those of ancestorRecord and serverRecord, to resolve the conflict.

The error’s `userInfo` dictionary contains the same value as this property. you can access it using the CKRecordChangedErrorClientRecordKey key.

## See Also

### Getting Conflicted Records

var ancestorRecord: CKRecord?

The original version of the record.

var serverRecord: CKRecord?

The server’s version of the record.

