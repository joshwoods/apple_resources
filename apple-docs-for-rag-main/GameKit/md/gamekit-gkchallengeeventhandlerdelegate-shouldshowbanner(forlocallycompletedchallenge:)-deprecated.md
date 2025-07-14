

- GameKit
- GKChallengeEventHandlerDelegate
-  shouldShowBanner(forLocallyCompletedChallenge:) Deprecated

Instance Method

# shouldShowBanner(forLocallyCompletedChallenge:)

Called to determine whether a banner should be shown when the local player completes a challenge.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func shouldShowBanner(forLocallyCompletedChallenge challenge: GKChallenge!) -> Bool
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

### Responding to Challenges Completed By the Local Player

func localPlayerDidComplete(GKChallenge!)

Called when the local player completes a challenge.

Deprecated

