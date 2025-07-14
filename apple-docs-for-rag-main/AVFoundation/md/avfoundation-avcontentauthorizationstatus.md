

- AVFoundation
-  AVContentAuthorizationStatus 

Enumeration

# AVContentAuthorizationStatus

A value representing the status of a content authorization request.

macOS

``` source
enum AVContentAuthorizationStatus
```

## Overview

Even if authorization is completed by the user, there is no guarantee that the content will then be authorized. You should re-check whether the content is authorized before proceeding.

## Topics

### Content Authorization Statuses

case unknown

The content authorization content request hasn’t completed.

case completed

The last completed call to request content authorization completed.

case cancelled

The last call to request content authorization was cancelled by the user.

case timedOut

The last call to request content authorization was cancelled because the timeout interval was reached.

case busy

The last call to request content authorization couldn’t be completed because another asset is currently attempting authorization.

case notAvailable

The last call to request content authorization couldn’t be completed because there was no known mechanism by which to attempt authorization.

case notPossible

The last call to request content authorization couldn’t be completed in a non-recoverable way.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Playback Authorization in macOS

var isContentAuthorizedForPlayback: Bool

A Boolean value that indicates whether the content has been authorized by the user.

var isAuthorizationRequiredForPlayback: Bool

A Boolean value that indicates whether authorization is required to play the content.

var isApplicationAuthorizedForPlayback: Bool

A Boolean value that indicates whether the application can be used to play the content.

func requestContentAuthorizationAsynchronously(withTimeoutInterval: TimeInterval, completionHandler: () -> Void)

Presents the user the opportunity to authorize the content for playback.

var contentAuthorizationRequestStatus: AVContentAuthorizationStatus

The status of the most recent content authorization request.

func cancelContentAuthorizationRequest()

Cancels the currently outstanding content authorization request.

