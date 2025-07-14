

- CloudKit
- CKModifyRecordsOperation
- CKModifyRecordsOperation.RecordSavePolicy
-  CKModifyRecordsOperation.RecordSavePolicy.allKeys 

Case

# CKModifyRecordsOperation.RecordSavePolicy.allKeys

A policy that instructs CloudKit to save all keys of a record, even those without changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
case allKeys
```

## Discussion

Important

This policy doesn’t compare record change tags. To ensure that you only save changes to the most recent version of a record, use CKModifyRecordsOperation.RecordSavePolicy.ifServerRecordUnchanged instead.

This policy causes CloudKit to overwrite any existing values on the server. It’s possible for a server record to contain keys that aren’t present locally. Another client might add keys to the record after you fetch it. Also, if you use the desiredKeys property to request a subset of keys during a fetch operation, saving that same record modifies only those keys that you include in the fetch and any keys you add to the record after that.

## See Also

### Save Policies

case ifServerRecordUnchanged

A policy that instructs CloudKit to only proceed if the record’s change tag matches that of the server’s copy.

case changedKeys

A policy that instructs CloudKit to save only the fields of a record that contain changes.

