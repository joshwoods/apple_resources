

- GameKit
- GKChallengeEventHandlerDelegate
-  localPlayerDidSelect(\_:) Deprecated

Instance Method

# localPlayerDidSelect(\_:)

Called when the local player selects a challenge banner displayed by GameKit.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func localPlayerDidSelect(_ challenge: GKChallenge!)
```

Deprecated

You should instead implement the GKChallengeListener protocol and register a listener with GKLocalPlayer.

## Parameters 

`challenge`  

The selected challenge.

