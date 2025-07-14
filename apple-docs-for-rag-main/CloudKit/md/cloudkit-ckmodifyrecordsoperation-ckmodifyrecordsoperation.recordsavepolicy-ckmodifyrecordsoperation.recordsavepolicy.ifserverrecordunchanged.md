

- CloudKit
- CKModifyRecordsOperation
- CKModifyRecordsOperation.RecordSavePolicy
-  CKModifyRecordsOperation.RecordSavePolicy.ifServerRecordUnchanged 

Case

# CKModifyRecordsOperation.RecordSavePolicy.ifServerRecordUnchanged

A policy that instructs CloudKit to only proceed if the record’s change tag matches that of the server’s copy.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
case ifServerRecordUnchanged
```

## Discussion

The server maintains a change tag for each record automatically. When you fetch a record, that change tag accompanies the rest of the record’s data. If the change tag in your local record matches the change tag of the record on the server, the save operation proceeds normally. If the server record contains a newer change tag, CloudKit doesn’t save the record and reports a CKError.Code.serverRecordChanged error.

## See Also

### Save Policies

case changedKeys

A policy that instructs CloudKit to save only the fields of a record that contain changes.

case allKeys

A policy that instructs CloudKit to save all keys of a record, even those without changes.

