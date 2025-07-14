

- Media Player
- MPPlayableContentDelegate
-  playableContentManager(\_:didUpdate:) Deprecated

Instance Method

# playableContentManager(\_:didUpdate:)

Notifies the delegate that the playable content manager’s context information has changed.

iOS 8.4–14.0DeprecatediPadOS 8.4–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func playableContentManager(
    _ contentManager: MPPlayableContentManager,
    didUpdate context: MPPlayableContentManagerContext
)
```

Deprecated

Use CarPlay framework

## Parameters 

`contentManager`  

The content manager whose current context has changed.

`context`  

The new context of the content manager.

## Discussion

A playable content manager’s context provides information about the current playback environment of an external media player, such as whether that media player limits the amount of content to display. Use the content manager’s `context` property to examine attributes of the new context after the change.

