

- AVFoundation
- AVPlayerItem
-  requestContentAuthorizationAsynchronously(withTimeoutInterval:completionHandler:) 

Instance Method

# requestContentAuthorizationAsynchronously(withTimeoutInterval:completionHandler:)

Presents the user the opportunity to authorize the content for playback.

macOS 10.7+

``` source
@MainActor
func requestContentAuthorizationAsynchronously(
    withTimeoutInterval timeoutInterval: TimeInterval,
    completionHandler handler: @escaping () -> Void
)
```

``` source
@MainActor
func requestContentAuthorization(withTimeoutInterval timeoutInterval: TimeInterval) async
```

## Parameters 

`timeoutInterval`  

The maximum amount of time in seconds to wait for the user to authorize the content before calling the handler block with a timeout result.

`handler`  

The block to be called upon completion.

## Discussion

Calling this method will present the user with the opportunity to authorize the content (for example, by launching iTunes and prompting the user to enter their Apple ID and password).

When the user has taken action (or the timeout has elapsed), the completion handler is invoked. You determine the status of the authorization attempt by checking the value of the contentAuthorizationRequestStatus property.

Even if the status indicates a completed authorization, the content may still not be authorized (for example, if the user authorizes an Apple ID other than that associated with the content). You should re-check the value of contentAuthorizationRequestStatus to verify whether the content has actually been authorized before continuing. It is not necessary to call this method if the value of contentAuthorizationRequestStatus is already true.

## See Also

### Managing Playback Authorization in macOS

var isContentAuthorizedForPlayback: Bool

A Boolean value that indicates whether the content has been authorized by the user.

var isAuthorizationRequiredForPlayback: Bool

A Boolean value that indicates whether authorization is required to play the content.

var isApplicationAuthorizedForPlayback: Bool

A Boolean value that indicates whether the application can be used to play the content.

var contentAuthorizationRequestStatus: AVContentAuthorizationStatus

The status of the most recent content authorization request.

enum AVContentAuthorizationStatus

A value representing the status of a content authorization request.

func cancelContentAuthorizationRequest()

Cancels the currently outstanding content authorization request.

