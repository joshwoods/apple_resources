

- Foundation
- URL Loading System
-  URL Loading System error info keys 

API Collection

# URL Loading System error info keys

Recognize these keys from the user info dictionary of error objects produced by URL Loading APIs.

## Overview

These keys are only present in the NSURLErrorDomain.

## Topics

### Keys

let NSURLErrorFailingURLErrorKey: String

The URL which caused a load to fail.

let NSURLErrorFailingURLPeerTrustErrorKey: String

The state of a failed SSL handshake.

let NSURLErrorFailingURLStringErrorKey: String

The URL which caused a load to fail.

Deprecated

let NSURLErrorBackgroundTaskCancelledReasonKey: String

A key in the error dictionary that provides the reason for canceling a background task.

URL Session Background Task Cancellation Reasons

Reasons that indicate why the system canceled a background task.

let NSURLErrorNetworkUnavailableReasonKey: String

The reason the network was unavailable for a task.

enum NetworkUnavailableReason

An enumeration of reasons explaining why a task couldn’t satisfy networking constraints.

### Deprecated

let NSErrorFailingURLStringKey: String

The URL that caused the error.

Deprecated

## See Also

### Errors

struct URLError

Error codes returned by URL loading APIs.

