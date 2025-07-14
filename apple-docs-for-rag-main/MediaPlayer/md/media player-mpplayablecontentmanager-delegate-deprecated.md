

- Media Player
- MPPlayableContentManager
-  delegate Deprecated

Instance Property

# delegate

A delegate that lets the media player manage the app’s playback queue.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
weak var delegate: (any MPPlayableContentDelegate)? { get set }
```

Deprecated

Use CarPlay framework

## Discussion

The delegate responds to external events that trigger a change in the media item that’s playing. An example of such an event would be choosing to play a song from a different album, or requesting suggested content to play next. The app must be able to respond to these events at any time.

To instead respond to events that affect the playback state of the currently playing item, use the MPRemoteCommandEvent class.

## See Also

### Responding to playback events

protocol MPPlayableContentDelegate

The protocol used to let external media players send playback commands to an app.

Deprecated

