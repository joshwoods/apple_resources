

- CloudKit
- CKSystemSharingUIObserver
-  systemSharingUIDidStopSharingBlock 

Instance Property

# systemSharingUIDidStopSharingBlock

A callback block the system invokes after the success or failure of a system sharing UI delete.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS

``` source
@preconcurrency
var systemSharingUIDidStopSharingBlock: ((CKRecord.ID, Result) -> Void)? { get set }
```

## Discussion

The system invokes this block on the success or failure of a CKShare delete when the user decides to stop sharing through the system sharing UI.

Each CKSystemSharingUIObserver instance has a private serial queue. The system uses this queue for all callback block invocations.

## See Also

### Accessing sharing blocks

var systemSharingUIDidSaveShareBlock: ((CKRecord.ID, Result&lt;CKShare, any Error>) -> Void)?

A callback block the system invokes after the success or failure of a system sharing UI save.

