

- WatchKit
- Storyboard support
-  Adding a Now Playing View 

Article

# Adding a Now Playing View

Provide a view that controls the currently playing audio from your app.

## Overview

With a Now Playing view, users can control current or recently played audio without leaving your app. When your app presents the Now Playing view, it immediately displays information about the current audio source, such as another app on the user’s Apple Watch or iPhone. For example, users can play and pause music from their Apple Watch’s Music app or control the volume of a podcast on their iPhone.

The system automatically selects the source. If the user is listening to audio on their watch or phone, the system selects that audio source. Otherwise, the system selects the most recently used source.

### Add the View to Your Storyboard

To add the Now Playing view, drag it from the Library to an empty interface controller in your WatchKit app’s storyboard.

Always present the Now Playing view so that it fills the screen in a nonscrolling container. Don’t add any other elements to this scene.

Note

If you are using SwiftUI, use the NowPlayingView structure instead.

The Now Playing view uses your app’s tint color, but otherwise has no attributes or properties that you can set. In addition, no public interface class exists for the Now Playing view. This means you can’t access or control the view programmatically. Your app just presents the view; the system handles the rest.

## See Also

### Audio

Playing Background Audio

Enable background audio in your app to provide a seamless playback experience.

class WKInterfaceVolumeControl

An interface element that provides control of the audio volume from the watch or a paired iPhone.

PUICAutoLaunchAudioOptOut

A Boolean value that indicates whether a watchOS app should opt out of automatically launching when its companion iOS app starts playing audio content.

class WKAudioFilePlayer

An object that controls playback of a single audio item.

Deprecated

class WKAudioFileQueuePlayer

An object that controls playback of one or more audio items.

Deprecated

class WKAudioFilePlayerItem

An object that manages the presentation state of an audio file while it is playing.

Deprecated

class WKAudioFileAsset

An object that stores a reference to an audio file and provides metadata information about that file.

Deprecated

