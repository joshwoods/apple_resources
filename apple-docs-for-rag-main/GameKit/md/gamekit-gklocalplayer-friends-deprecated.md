

- GameKit
- GKLocalPlayer
-  friends Deprecated

Instance Property

# friends

The player identifiers for the local player’s friends.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var friends: [String]? { get }
```

Deprecated

Use loadFriendPlayers(completionHandler:) instead.

## Discussion

This property is invalid until a call to loadFriendsObsoleted(completionHandler:) succeeds.

