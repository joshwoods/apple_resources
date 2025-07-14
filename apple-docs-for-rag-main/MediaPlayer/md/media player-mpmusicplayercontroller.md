

- Media Player
-  MPMusicPlayerController 

Class

# MPMusicPlayerController

An object that plays audio media items from the device’s Music app library.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class MPMusicPlayerController
```

## Mentioned in 

Playing audio using the built-in music player

## Overview

Create an instance of a music player to play media items in your app. There are two types of music players:

- An *application music player* plays music locally within your app. It isn’t aware of the Music app’s Now Playing item, nor does it affect the Music app’s state. There are two application music players: applicationMusicPlayer and applicationQueuePlayer. The application queue player provides greater control over the contents of the queue and is the preferred player.

- The *system music player* employs the built-in Music app on your behalf. On instantiation, it takes on the current Music app state, such as the identification of the Now Playing item. If a user switches away from your app while music is playing, that music continues to play. The Music app then has your music player’s most recently-set repeat mode, shuffle mode, playback state, and Now Playing item.

Creating a new instance of `MPMusicPlayerController` and not specifying the player type returns a system music player.

Important

Only use a music player on the app’s main thread.

### Accessing limited playback information while using Home Sharing

The built-in Music and Videos apps can play media from shared libraries using Home Sharing. However, third-party apps using the Media Player framework only have access to the device music library. This means that your app can’t display the title of a home-shared song in your user interface. Specifically, if the Music app is playing a home-shared song, and you’re using a system music player, the value of the nowPlayingItem property of your music player is nil. However, other playback information is available when playing shared media. For example, the framework updates the value of the playbackState property when the system music player plays a home-shared item.

### Choosing how the system handles remote control events

Users can initiate audio playback commands through an external headset or accessory.

- If you use an *application music player*, the system sends these commands as remote control events to your app, but you don’t provide code to handle them. The framework receives and handles the remote control events.

- If you use the *system music player*, your app uses the Music app to play audio, which means that the Music app is the Now Playing app. The Music app receives and handles the remote control events. For example, if your app plays audio using the system music player, and the user switches from your app to the iOS device’s Now Playing controls, the controls work as expected. That is, they can play or pause audio, or skip to the next and previous items.

## Topics

### Getting a music player

class var applicationMusicPlayer: MPMusicPlayerController

Returns the application music player.

class var applicationQueuePlayer: MPMusicPlayerApplicationController

Returns the application queue music player.

class var systemMusicPlayer: any MPMusicPlayerController &amp; MPSystemMusicPlayerController

Returns the system music player, which controls the Music app’s state.

### Setting up a playback queue

Before a music player can produce sound, it needs a playback queue. You provide the music player with its playback queue, which specifies the media items to play.

func setQueue(with: MPMediaQuery)

Sets a music player’s playback queue based on a media query.

func setQueue(with: MPMediaItemCollection)

Sets a music player’s playback queue using a media item collection.

func setQueue(with: [String])

Sets a music player’s playback queue using with media items identified by the store identifiers.

func setQueue(with: MPMusicPlayerQueueDescriptor)

Set the music player’s playback queue using media items that fit the queue descriptor properties.

### Playing a media item

func prepareToPlay(completionHandler: ((any Error)?) -> Void)

Prepares a music player for playback.

### Managing playback mode and state

var nowPlayingItem: MPMediaItem?

The currently-playing media item, or the media item in a queue that you designated to begin playback with.

var indexOfNowPlayingItem: Int

The index of the now playing item in the current playback queue.

var playbackState: MPMusicPlaybackState

The current playback state of the music player.

var repeatMode: MPMusicRepeatMode

The current repeat mode of the music player.

var shuffleMode: MPMusicShuffleMode

The current shuffle mode of the music player.

enum MPMusicPlaybackState

The music player playback state modes.

enum MPMusicRepeatMode

The repeat modes for the media player.

enum MPMusicShuffleMode

The shuffle modes for the media player.

var volume: Float

The audio playback volume for the music player, in the range from `0.0` (silent) through `1.0` (maximum volume).

Deprecated

### Controlling playback

func skipToNextItem()

Starts playback of the next media item in the playback queue, or if the music player isn’t playing, designates the next media item as the next item to play.

func skipToBeginning()

Restarts playback at the beginning of the currently playing media item.

func skipToPreviousItem()

Starts playback of the previous media item in the playback queue, or if the music player isn’t playing, designates the previous media item as the next to play.

func append(MPMusicPlayerQueueDescriptor)

Inserts the media items defined by the queue descriptor after the last media item in the current queue.

func prepend(MPMusicPlayerQueueDescriptor)

Inserts the media items defined by the queue descriptor into the current queue immediately after the currently playing media item.

### Using music player notifications

These methods control the posting of playback notifications. You can nest calls to start or end these notifications.

func beginGeneratingPlaybackNotifications()

Starts the generation of playback notifications.

func endGeneratingPlaybackNotifications()

Ends the generation of playback notifications.

### Type Properties

class var iPodMusicPlayer: MPMusicPlayerController

Returns the iPod music player, which controls the iPod app’s state.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- MPMusicPlayerApplicationController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MPMediaPlayback
- NSObjectProtocol

## See Also

### Built-in music playback

Playing audio using the built-in music player

Create a media player inside your app to play audio from the user’s media library.

protocol MPMediaPlayback

A protocol that defines the interface for controlling audio media playback.

protocol MPSystemMusicPlayerController

A protocol for playing videos in the Music app.

