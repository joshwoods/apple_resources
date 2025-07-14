

- Media Player
-  MPNowPlayingInfoPropertyElapsedPlaybackTime 

Global Variable

# MPNowPlayingInfoPropertyElapsedPlaybackTime

The elapsed time of the Now Playing item, in seconds.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.12.2+tvOSvisionOS 1.0+watchOS 5.0+

``` source
let MPNowPlayingInfoPropertyElapsedPlaybackTime: String
```

## Discussion

Value is an NSNumber object configured as a `double`. Elapsed time is automatically calculated, by the system, from the previously provided elapsed time and the playback rate. It isn’t necessary to update this property frequently.

## See Also

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

