

- AVFoundation
- AVPlayerItem
-  contentAuthorizationRequestStatus 

Instance Property

# contentAuthorizationRequestStatus

The status of the most recent content authorization request.

macOS 10.7+

``` source
@MainActor
var contentAuthorizationRequestStatus: AVContentAuthorizationStatus { get }
```

## Discussion

This property reports the authorization status as determined by the most recent call to requestContentAuthorizationAsynchronously(withTimeoutInterval:completionHandler:).

The value will be AVContentAuthorizationStatus.unknown before the first call and between the time a request call is made and just prior to the completion handler being executed (thus it is safe to query this property from the completion handler).

This value is not key-value observable.

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

enum AVContentAuthorizationStatus

A value representing the status of a content authorization request.

func cancelContentAuthorizationRequest()

Cancels the currently outstanding content authorization request.

