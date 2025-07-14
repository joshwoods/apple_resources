

- GameKit
- GKChallengeEventHandlerDelegate
-  localPlayerDidComplete(\_:) Deprecated

Instance Method

# localPlayerDidComplete(\_:)

Called when the local player completes a challenge.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func localPlayerDidComplete(_ challenge: GKChallenge!)
```

Deprecated

You should instead implement the GKChallengeListener protocol and register a listener with GKLocalPlayer.

## Parameters 

`challenge`  

The completed challenge.

## See Also

### Responding to Challenges Completed By the Local Player

func shouldShowBanner(forLocallyCompletedChallenge: GKChallenge!) -> Bool

Called to determine whether a banner should be shown when the local player completes a challenge.

Deprecated

