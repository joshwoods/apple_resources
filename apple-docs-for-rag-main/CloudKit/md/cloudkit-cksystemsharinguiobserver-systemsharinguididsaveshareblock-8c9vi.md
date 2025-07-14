

- CloudKit
- CKSystemSharingUIObserver
-  systemSharingUIDidSaveShareBlock 

Instance Property

# systemSharingUIDidSaveShareBlock

A callback block the system invokes after the success or failure of a system sharing UI save.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS

``` source
@preconcurrency
var systemSharingUIDidSaveShareBlock: ((CKRecord.ID, Result) -> Void)? { get set }
```

## Discussion

Following a successful share save by the system sharing UI in the provided CKContainer, the system invokes this callback with a `nonnull` CKRecord.ID, a `nonnull` share, and a `nil` error.

If a save failure occurs due to a per-item error like CKError.Code.serverRecordChanged, the system invokes this callback with a `nonnull` `CKRecord.ID`, a `nil` share, and a `nonnull` error.

Each CKSystemSharingUIObserver instance has a private serial queue. The system uses this queue for all callback block invocations.

## See Also

### Accessing sharing blocks

var systemSharingUIDidStopSharingBlock: ((CKRecord.ID, Result&lt;Void, any Error>) -> Void)?

A callback block the system invokes after the success or failure of a system sharing UI delete.

