

- AVFoundation
- AVPlayerItem
-  requestPlaybackRestrictionsAuthorization(\_:) 

Instance Method

# requestPlaybackRestrictionsAuthorization(\_:)

Determines whether this item is subject to parental restrictions, and, if so, prompts the user to enter the restrictions passcode.

tvOS 13.0+

``` source
@MainActor
func requestPlaybackRestrictionsAuthorization(_ completion: @escaping (Bool, (any Error)?) -> Void)
```

``` source
@MainActor
func requestPlaybackRestrictionsAuthorization() async throws -> Bool
```

## Parameters 

`completion`  

A callback the system invokes after it makes a determination of parental restrictions.

`isAuthorized`  
A Boolean value that indicates whether the system authorizes the app to play an item.

`error`  
An optional error that contains error details if the system encountered an error.

## See Also

### Requesting Playback Authorization in tvOS

func cancelPlaybackRestrictionsAuthorizationRequest()

Cancels a pending authorization request and dismisses the passcode entry, if displayed.

