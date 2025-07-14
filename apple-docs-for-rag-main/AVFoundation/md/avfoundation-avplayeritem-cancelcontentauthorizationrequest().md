

- AVFoundation
- AVPlayerItem
-  cancelContentAuthorizationRequest() 

Instance Method

# cancelContentAuthorizationRequest()

Cancels the currently outstanding content authorization request.

macOS 10.7+

``` source
@MainActor
func cancelContentAuthorizationRequest()
```

## Discussion

Calling this method while a content authorization request is pending will cause that request to be cancelled and its completion handler to be invoked with a status of AVContentAuthorizationStatus.cancelled.

This method does not block.

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

enum AVContentAuthorizationStatus

A value representing the status of a content authorization request.

