

- AVFoundation
- AVPlayerItem
-  isApplicationAuthorizedForPlayback 

Instance Property

# isApplicationAuthorizedForPlayback

A Boolean value that indicates whether the application can be used to play the content.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.7+

``` source
@MainActor
var isApplicationAuthorizedForPlayback: Bool { get }
```

## Discussion

This property reports whether or not the calling application is authorized to play the content associated with the item.

Application authorization is independent of content authorization (see isContentAuthorizedForPlayback) and that both must be granted in order for an application to be allowed to play protected content. Also, unlike content authorization, application authorization is not dependent on user credentials (that is, if `applicationAuthorizedForPlayback` is false, there are no means to obtain authorization).

This property is not key-value observable.

## See Also

### Managing Playback Authorization in macOS

var isContentAuthorizedForPlayback: Bool

A Boolean value that indicates whether the content has been authorized by the user.

var isAuthorizationRequiredForPlayback: Bool

A Boolean value that indicates whether authorization is required to play the content.

func requestContentAuthorizationAsynchronously(withTimeoutInterval: TimeInterval, completionHandler: () -> Void)

Presents the user the opportunity to authorize the content for playback.

var contentAuthorizationRequestStatus: AVContentAuthorizationStatus

The status of the most recent content authorization request.

enum AVContentAuthorizationStatus

A value representing the status of a content authorization request.

func cancelContentAuthorizationRequest()

Cancels the currently outstanding content authorization request.

