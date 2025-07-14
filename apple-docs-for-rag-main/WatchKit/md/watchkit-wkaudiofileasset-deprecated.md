

- WatchKit
-  WKAudioFileAsset Deprecated

Class

# WKAudioFileAsset

An object that stores a reference to an audio file and provides metadata information about that file.

watchOS 2.0–6.0Deprecated

``` source
class WKAudioFileAsset
```

Deprecated

Use the AVFoundation framework’s AVPlayer and AVQueuePlayer classes instead.

## Overview

You create assets when you want to play audio from your watchOS app. Use the audio file asset object to store the location of the file and any Now Playing information you want displayed while the audio is playing.

Audio assets must refer to files on the local file system. If you have audio files that are stored on a server, you must download them to the user’s Apple Watch before attempting to play them using an audio file asset object.

It is recommended that you encode audio files using 32 kbps stereo AAC. You may use other bit rates, or the LPCM encoding, as preferred for your content.

To play an audio file asset, wrap it in a WKAudioFilePlayerItem object. The player item object stores information about the playback status of the asset and works with a WKAudioFilePlayer object to coordinate playback. If you want to queue several audio files for playback, you manage those items using a WKAudioFileQueuePlayer object.

## Topics

### Creating an Asset

convenience init(url: URL)

Returns an asset for the audio file at the specified URL.

convenience init(url: URL, title: String?, albumTitle: String?, artist: String?)

Returns an audio file asset and sets the metadata for that item.

### Getting the Asset’s Properties

var url: URL

The URL of the audio file.

var duration: TimeInterval

The duration (in seconds) of the audio file.

var title: String?

The title information for the audio file.

var albumTitle: String?

The album title information for the audio file.

var artist: String?

The artist information for the audio file.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio

Playing Background Audio

Enable background audio in your app to provide a seamless playback experience.

Adding a Now Playing View

Provide a view that controls the currently playing audio from your app.

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

