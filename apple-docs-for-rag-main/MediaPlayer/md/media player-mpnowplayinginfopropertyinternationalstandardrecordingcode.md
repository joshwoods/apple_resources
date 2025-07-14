

- Media Player
-  MPNowPlayingInfoPropertyInternationalStandardRecordingCode 

Global Variable

# MPNowPlayingInfoPropertyInternationalStandardRecordingCode

The International Standard Recording Code (ISRC) of the Now Playing item.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
let MPNowPlayingInfoPropertyInternationalStandardRecordingCode: String
```

## Discussion

The value is a string that represents the International Standard Recording Code (ISRC) for a song, if one is available. System services that leverage Now Playing data, such as Music Haptics, use this value. For more information, read Music Haptics.

## See Also

### Related Documentation

Music Haptics

Play haptic tracks along with known music tracks.

### Accessing Now Playing metadata properties

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

let MPNowPlayingInfoPropertyIsLiveStream: String

A number that denotes whether the Now Playing item is a live stream.

