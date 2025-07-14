

- Foundation
-  NSCloudSharingOtherError 

Global Variable

# NSCloudSharingOtherError

An otherwise unspecified cloud-sharing error occurred.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+

``` source
var NSCloudSharingOtherError: Int { get }
```

## Discussion

For CloudKit sharing, use the NSUnderlyingErrorKey, whose value is a CKErrorDomain error, to discover the specific error. Refer to the CloudKit documentation for the proper response to these errors.

## See Also

### iCloud Sharing Errors

var NSCloudSharingConflictError: Int

A conflict occurred during an attempt to save changes.

var NSCloudSharingErrorMaximum: Int

The end of the range of error codes reserved for cloud-sharing errors.

var NSCloudSharingErrorMinimum: Int

The start of the range of error codes reserved for cloud-sharing errors.

var NSCloudSharingNetworkFailureError: Int

Sharing failed due to a network failure.

var NSCloudSharingNoPermissionError: Int

The current user doesn’t have permission to perform the requested actions.

var NSCloudSharingQuotaExceededError: Int

The user doesn’t have enough storage space available to share the requested items.

var NSCloudSharingTooManyParticipantsError: Int

Additional participants couldn’t be added to the share, because the limit was reached.

