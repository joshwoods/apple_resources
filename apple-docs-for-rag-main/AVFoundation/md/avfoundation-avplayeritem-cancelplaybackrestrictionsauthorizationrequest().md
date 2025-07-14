

- AVFoundation
- AVPlayerItem
-  cancelPlaybackRestrictionsAuthorizationRequest() 

Instance Method

# cancelPlaybackRestrictionsAuthorizationRequest()

Cancels a pending authorization request and dismisses the passcode entry, if displayed.

tvOS 13.0+

``` source
@MainActor
func cancelPlaybackRestrictionsAuthorizationRequest()
```

## See Also

### Requesting Playback Authorization in tvOS

func requestPlaybackRestrictionsAuthorization((Bool, (any Error)?) -> Void)

Determines whether this item is subject to parental restrictions, and, if so, prompts the user to enter the restrictions passcode.

