

- AVFoundation
- AVPlayerItem
-  isContentAuthorizedForPlayback 

Instance Property

# isContentAuthorizedForPlayback

A Boolean value that indicates whether the content has been authorized by the user.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.7+

``` source
@MainActor
var isContentAuthorizedForPlayback: Bool { get }
```

## Discussion

This property reports whether the user has provided the necessary credentials to the system in order for the content to be decrypted for playback.

Content authorization is independent of application authorization (see isApplicationAuthorizedForPlayback) and that both must be granted in order for an application to be allowed to play protected content.

This property is not key-value observable.

## See Also

### Managing Playback Authorization in macOS

var isAuthorizationRequiredForPlayback: Bool

A Boolean value that indicates whether authorization is required to play the content.

var isApplicationAuthorizedForPlayback: Bool

A Boolean value that indicates whether the application can be used to play the content.

func requestContentAuthorizationAsynchronously(withTimeoutInterval: TimeInterval, completionHandler: () -> Void)

Presents the user the opportunity to authorize the content for playback.

var contentAuthorizationRequestStatus: AVContentAuthorizationStatus

The status of the most recent content authorization request.

enum AVContentAuthorizationStatus

A value representing the status of a content authorization request.

func cancelContentAuthorizationRequest()

Cancels the currently outstanding content authorization request.

