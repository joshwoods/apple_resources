

- Foundation
- URL Loading System
- URLSession
-  Background task cancellation 

API Collection

# Background task cancellation

Constants that indicate why a background task was canceled.

## Overview

These values are used in conjunction with the NSURLErrorBackgroundTaskCancelledReasonKey key in an NSError object’s `userInfo` dictionary.

## Topics

### Cancellation reasons

var NSURLErrorCancelledReasonBackgroundUpdatesDisabled: Int

A reason that indicates the system canceled the background task because background tasks are disabled.

var NSURLErrorCancelledReasonInsufficientSystemResources: Int

A reason that indicates the system canceled the background task because it lacks sufficient resources to perform the task.

var NSURLErrorCancelledReasonUserForceQuitApplication: Int

A reason that indicates the system canceled the background task because the user force-quit the application.

## See Also

### Handling errors

URL session error dictionary keys

Keys used in conjunction with error objects returned by URL sessions and tasks.

