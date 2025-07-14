

- Media Player
-  MPPlayableContentDelegate Deprecated

Protocol

# MPPlayableContentDelegate

The protocol used to let external media players send playback commands to an app.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
protocol MPPlayableContentDelegate : NSObjectProtocol
```

Deprecated

Use CarPlay framework

## Overview

After the media player determines that a media item should play, the app’s content delegate requests to initiate playback.

Important

Some features of this protocol are specific to CarPlay, which requires a special entitlement issued by Apple. Apps without the correct entitlement won’t appear on the CarPlay home screen. See http://www.apple.com/ios/carplay/ for more information.

When creating your CarPlay app, keep the following in mind:

- Transition to the Now Playing screen only when content is ready to play. Due to buffering and network conditions, it may take several seconds for audio to begin playing after a user selects it. The user’s selection remains highlighted, and the system displays a spinning activity indicator until your app informs the system that the audio is ready to play.

- Start playback as soon as possible. Playback should begin as soon as audio has sufficiently loaded, even if descriptive information is still loading. Continue loading descriptive information in the background and show it once available.

- Avoid beginning playback automatically. Unless your app’s purpose is to play a single source of audio, it shouldn’t begin playback until the user initiates it.

## Topics

### Playing a specific media item

func playableContentManager(MPPlayableContentManager, initiatePlaybackOfContentItemAt: IndexPath, completionHandler: ((any Error)?) -> Void)

Asks the delegate to begin playback of the specified content item.

### Suggesting content for playback

func playableContentManager(MPPlayableContentManager, initializePlaybackQueueWithContentItems: [Any]?, completionHandler: ((any Error)?) -> Void)

Asks the delegate to prepare suggested content for playback.

func playableContentManager(MPPlayableContentManager, initializePlaybackQueueWithCompletionHandler: ((any Error)?) -> Void)

Asks the delegate to prepare suggested content for playback.

### Responding to context changes

func playableContentManager(MPPlayableContentManager, didUpdate: MPPlayableContentManagerContext)

Notifies the delegate that the playable content manager’s context information has changed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to playback events

var delegate: (any MPPlayableContentDelegate)?

A delegate that lets the media player manage the app’s playback queue.

Deprecated

