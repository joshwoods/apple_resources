

- CloudKit
- CKModifyRecordsOperation
- CKModifyRecordsOperation.RecordSavePolicy
-  CKModifyRecordsOperation.RecordSavePolicy.changedKeys 

Case

# CKModifyRecordsOperation.RecordSavePolicy.changedKeys

A policy that instructs CloudKit to save only the fields of a record that contain changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
case changedKeys
```

## Discussion

Important

This policy doesn’t compare record change tags. To ensure that you only save changes to the most recent version of a record, use CKModifyRecordsOperation.RecordSavePolicy.ifServerRecordUnchanged instead.

## See Also

### Save Policies

case ifServerRecordUnchanged

A policy that instructs CloudKit to only proceed if the record’s change tag matches that of the server’s copy.

case allKeys

A policy that instructs CloudKit to save all keys of a record, even those without changes.

