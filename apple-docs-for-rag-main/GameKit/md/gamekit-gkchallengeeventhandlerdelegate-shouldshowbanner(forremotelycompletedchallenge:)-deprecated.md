

- GameKit
- GKChallengeEventHandlerDelegate
-  shouldShowBanner(forRemotelyCompletedChallenge:) Deprecated

Instance Method

# shouldShowBanner(forRemotelyCompletedChallenge:)

Called to determine whether a banner should be shown when a remote player completes a challenge.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func shouldShowBanner(forRemotelyCompletedChallenge challenge: GKChallenge!) -> Bool
```

Deprecated

You should instead implement the GKChallengeListener protocol and register a listener with GKLocalPlayer.

## Parameters 

`challenge`  

The completed challenge.

## Return Value

Your delegate should return true if it wants a banner to be displayed. Otherwise it should return false.

## Discussion

If you do not implement this method, a banner is always shown.

## See Also

### Responding to Challenges Issued by the Local Player

func remotePlayerDidComplete(GKChallenge!)

Called when a remote player completes a challenge issued by the local player.

Deprecated

