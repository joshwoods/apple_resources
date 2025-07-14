

- Media Player
-  MPNowPlayingInfoPropertyPlaybackRate 

Global Variable

# MPNowPlayingInfoPropertyPlaybackRate

The playback rate of the Now Playing item.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.12.2+tvOSvisionOS 1.0+watchOS 5.0+

``` source
let MPNowPlayingInfoPropertyPlaybackRate: String
```

## Discussion

Value is an NSNumber object configured as a `double`. The default value is `1.0`, which indicates a normal playback rate. A playback rate value of `2.0` means twice the normal playback rate; a piece of media played at this rate would take half as long to play to completion. A value of `0.5` means half the normal playback rate; a piece of media played at this rate would take twice as long to play to completion.

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

