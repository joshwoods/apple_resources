

- GameKit
- GKChallengeEventHandlerDelegate
-  localPlayerDidReceive(\_:) Deprecated

Instance Method

# localPlayerDidReceive(\_:)

Called when the local player receives a new challenge.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func localPlayerDidReceive(_ challenge: GKChallenge!)
```

Deprecated

You should instead implement the GKChallengeListener protocol and register a listener with GKLocalPlayer.

## Parameters 

`challenge`  

The received challenge.

## See Also

### Responding When a New Challenge is Received

func shouldShowBanner(forLocallyReceivedChallenge: GKChallenge!) -> Bool

Called to determine whether a banner should be shown when the local player receives a challenge.

Deprecated

