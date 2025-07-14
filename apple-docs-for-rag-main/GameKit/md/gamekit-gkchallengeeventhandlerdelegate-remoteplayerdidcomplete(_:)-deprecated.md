

- GameKit
- GKChallengeEventHandlerDelegate
-  remotePlayerDidComplete(\_:) Deprecated

Instance Method

# remotePlayerDidComplete(\_:)

Called when a remote player completes a challenge issued by the local player.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func remotePlayerDidComplete(_ challenge: GKChallenge!)
```

Deprecated

You should instead implement the GKChallengeListener protocol and register a listener with GKLocalPlayer.

## Parameters 

`challenge`  

The completed challenge.

## See Also

### Responding to Challenges Issued by the Local Player

func shouldShowBanner(forRemotelyCompletedChallenge: GKChallenge!) -> Bool

Called to determine whether a banner should be shown when a remote player completes a challenge.

Deprecated

