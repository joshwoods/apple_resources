

- Foundation
-  NSCloudSharingConflictError 

Global Variable

# NSCloudSharingConflictError

A conflict occurred during an attempt to save changes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+

``` source
var NSCloudSharingConflictError: Int { get }
```

## Discussion

This error occurs when a conflict is detected while trying to save changes to the CKShare or root CKRecord. Respond to this error by first fetching the server’s changes to the records, then either handle the conflict manually or present it, which will instruct the user to try the operation again.

## See Also

### iCloud Sharing Errors

var NSCloudSharingErrorMaximum: Int

The end of the range of error codes reserved for cloud-sharing errors.

var NSCloudSharingErrorMinimum: Int

The start of the range of error codes reserved for cloud-sharing errors.

var NSCloudSharingNetworkFailureError: Int

Sharing failed due to a network failure.

var NSCloudSharingNoPermissionError: Int

The current user doesn’t have permission to perform the requested actions.

var NSCloudSharingOtherError: Int

An otherwise unspecified cloud-sharing error occurred.

var NSCloudSharingQuotaExceededError: Int

The user doesn’t have enough storage space available to share the requested items.

var NSCloudSharingTooManyParticipantsError: Int

Additional participants couldn’t be added to the share, because the limit was reached.

