

- CloudKit
- CKFetchShareParticipantsOperation
-  shareParticipantFetchedBlock Deprecated

Instance Property

# shareParticipantFetchedBlock

The closure to execute as the operation generates individual participants.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var shareParticipantFetchedBlock: ((CKShare.Participant) -> Void)? { get set }
```

Deprecated

Use perShareParticipantCompletionBlock instead, which surfaces per-share-participant errors

## Discussion

The closure returns no value and takes the following parameters:

- The participant that the operation generates.

The operation executes this closure once for each item of user data in the userIdentityLookupInfos property. Each time the closure executes, it executes serially with respect to the other closures of the operation.

If you intend to use this closure to process results, set it before you execute the operation or submit the operation to a queue.

## See Also

### Processing the Operation’s Results

var fetchShareParticipantsCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

Deprecated

