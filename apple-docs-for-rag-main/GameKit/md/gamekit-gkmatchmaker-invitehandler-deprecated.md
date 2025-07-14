

- GameKit
- GKMatchmaker
-  inviteHandler Deprecated

Instance Property

# inviteHandler

A block that GameKit calls when an invitation to join a match is accepted by the local player.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var inviteHandler: ((GKInvite, [Any]?) -> Void)? { get set }
```

Deprecated

Use the register(_:) method instead.

## Discussion

The block takes the following parameters:

*acceptedInvite*  
The invitation accepted by the player.

*playerIDsToInvite*  
An array of `NSString` objects containing player identifiers for additional players to invite into the game.

Your block needs to respond to the invitation in one of two ways:

- Display the standard user interface by initializing a new GKMatchmakerViewController object, passing the invitation object and the list of player identifiers as parameters.

- Create a match programmatically by calling the match(for:completionHandler:) method on the shared matchmaker instance.

If your game receives an invitation while it’s running, it needs to transition to multiplayer play. It must clean up any existing content, such as ending the current match the player is playing, and then process the invitation.

