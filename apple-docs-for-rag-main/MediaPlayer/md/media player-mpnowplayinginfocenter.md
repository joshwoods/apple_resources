

- Media Player
-  MPNowPlayingInfoCenter 

Class

# MPNowPlayingInfoCenter

An object for setting the Now Playing information for media that your app plays.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 5.0+visionOS 1.0+watchOS 5.0+

``` source
class MPNowPlayingInfoCenter
```

## Overview

If your app also provides Now Playing information containing information about the current track, use this object to update that information at appropriate times. This object contains a nowPlayingInfo dictionary describing the playing item.

Important

Siri can provide suggestions in search, News, Safari, and other apps using on-device information that you contribute through the Now Playing APIs. Users can control Siri on-device learning through Siri and Search settings for your app.

The system displays Now Playing information on the device’s Lock Screen and in the media controls in Control Center. If the user directs playback of your media to Apple TV using AirPlay, the Now Playing information appears on the television screen. If the user connects a device to an iPod accessory, such as in a car, the accessory may display Now Playing information.

Important

To ensure that your app interacts successfully with the widest possible range of accessories, provide values for as many information properties as you can in the nowPlayingInfo dictionary.

The information you can specify includes all of the Now Playing metadata properties (see the Accessing Now Playing metadata properties topic group below), and the following subset of MPMediaItem properties:

- MPMediaItemPropertyAlbumTitle

- MPMediaItemPropertyAlbumTrackCount

- MPMediaItemPropertyAlbumTrackNumber

- MPMediaItemPropertyArtist

- MPMediaItemPropertyArtwork

- MPMediaItemPropertyComposer

- MPMediaItemPropertyDiscCount

- MPMediaItemPropertyDiscNumber

- MPMediaItemPropertyGenre

- MPMediaItemPropertyMediaType

- MPMediaItemPropertyPersistentID

- MPMediaItemPropertyPlaybackDuration

- MPMediaItemPropertyTitle

You don’t have direct control over what information the system displays, or its formatting. You set the values in the nowPlayingInfo dictionary and the system or the connected accessory handles displaying the information in a consistent manner for all apps.

You can ensure that your app interacts well with other apps providing Now Playing information by following the best practices in the Becoming a now playable app sample code project.

Important

In iOS 17.2 and later, the Journal app encourages people to reflect and write about their day-to-day experiences, including media they listened to or watched. If your app donates media information to MPNowPlayingInfoCenter, and you choose not to opt-out, the media played may appear as a suggestion in the Journal app, or other apps that use the Journaling Suggestions framework.

## Topics

### Working with the default Now Playing info center

class func `default`() -> MPNowPlayingInfoCenter

Returns the singleton Now Playing info center.

var nowPlayingInfo: [String : Any]?

The current Now Playing information for the default Now Playing info center.

enum MPNowPlayingInfoMediaType

The type of media currently playing.

### Setting the playback state in macOS

var playbackState: MPNowPlayingPlaybackState

The current playback state of the app.

enum MPNowPlayingPlaybackState

The playback state of the app.

### Accessing Now Playing metadata properties

Provide specific details about the currently playing item.

let MPNowPlayingInfoCollectionIdentifier: String

The identifier of the collection the Now Playing item belongs to.

let MPNowPlayingInfoPropertyAdTimeRanges: String

A list of ad breaks in the Now Playing item.

let MPNowPlayingInfoPropertyAvailableLanguageOptions: String

The available language option groups for the Now Playing item.

let MPNowPlayingInfoPropertyAssetURL: String

The URL pointing to the Now Playing item’s underlying asset.

let MPNowPlayingInfoPropertyChapterCount: String

The total number of chapters in the Now Playing item.

let MPNowPlayingInfoPropertyChapterNumber: String

The number corresponding to the currently playing chapter.

let MPNowPlayingInfoPropertyCreditsStartTime: String

The start time for the credits, in seconds, without ads, for the Now Playing item.

let MPNowPlayingInfoPropertyCurrentLanguageOptions: String

The currently active language options for the Now Playing item.

let MPNowPlayingInfoPropertyCurrentPlaybackDate: String

The date associated with the current elapsed playback time.

let MPNowPlayingInfoPropertyDefaultPlaybackRate: String

The default playback rate for the Now Playing item.

let MPNowPlayingInfoPropertyElapsedPlaybackTime: String

The elapsed time of the Now Playing item, in seconds.

let MPNowPlayingInfoPropertyExcludeFromSuggestions: String

A number that denotes whether to exclude the Now Playing item from content suggestions.

let MPNowPlayingInfoPropertyExternalContentIdentifier: String

The opaque identifier that uniquely identifies the Now Playing item, even through app relaunches.

let MPNowPlayingInfoPropertyExternalUserProfileIdentifier: String

The opaque identifier that uniquely identifies the profile the Now Playing item plays from, even through app relaunches.

let MPNowPlayingInfoPropertyInternationalStandardRecordingCode: String

The International Standard Recording Code (ISRC) of the Now Playing item.

let MPNowPlayingInfoPropertyIsLiveStream: String

A number that denotes whether the Now Playing item is a live stream.

let MPNowPlayingInfoPropertyMediaType: String

The media type of the Now Playing item.

let MPNowPlayingInfoPropertyPlaybackProgress: String

The current progress of the Now Playing item.

let MPNowPlayingInfoPropertyPlaybackRate: String

The playback rate of the Now Playing item.

let MPNowPlayingInfoPropertyPlaybackQueueCount: String

The total number of items in the app’s playback queue.

let MPNowPlayingInfoPropertyPlaybackQueueIndex: String

The index of the Now Playing item in the app’s playback queue.

let MPNowPlayingInfoPropertyServiceIdentifier: String

The service provider associated with the Now Playing item.

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

### Now Playing information

Becoming a now playable app

Ensure your app is eligible to become the Now Playing app by adopting best practices for providing Now Playing info and registering for remote command center actions.

class MPNowPlayingSession

An object that manages Now Playing information and remote commands for multiple players.

class MPNowPlayingInfoLanguageOption

A set of interfaces for setting the language option for the Now Playing item.

class MPNowPlayingInfoLanguageOptionGroup

A grouped set of language options where only a single language option can be active at a time.

Language option characteristic constants

The constants for defining language characteristics.

