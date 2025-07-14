

- GameKit
- GKMatch
-  voiceChat(withName:) Deprecated

Instance Method

# voiceChat(withName:)

Joins the local player to a voice channel.

iOS 4.1–18.0DeprecatediPadOS 4.1–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func voiceChat(withName name: String) -> GKVoiceChat?
```

Deprecated

No longer supported

## Parameters 

`name`  

The name of the channel to join.

## Return Value

A voice chat object for the channel, or `nil` if an error occurs or parental controls restrict the player from joining a voice chat.

## Discussion

This method adds the local player to the named voice chat channel and creates it if necessary. GameKit connects players who join a channel with the same name. A match can have multiple channels and a player can join multiple channels.

When the local player disconnects from a match, all voice channels associated with the match stop working. Therefore, before you disconnect a player, you need to stop the associated voice channels and set the voice chat objects to `nil`.

