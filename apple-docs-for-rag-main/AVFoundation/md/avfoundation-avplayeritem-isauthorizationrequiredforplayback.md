

- AVFoundation
- AVPlayerItem
-  isAuthorizationRequiredForPlayback 

Instance Property

# isAuthorizationRequiredForPlayback

A Boolean value that indicates whether authorization is required to play the content.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.7+

``` source
@MainActor
var isAuthorizationRequiredForPlayback: Bool { get }
```

## Discussion

This property reports whether authorization is required for the item’s content to be played. If it does not require authorization, then none of the other authorization-related methods or properties apply (though they will return sensible values where possible).

This property is not key-value observable.

## See Also

### Managing Playback Authorization in macOS

var isContentAuthorizedForPlayback: Bool

A Boolean value that indicates whether the content has been authorized by the user.

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

