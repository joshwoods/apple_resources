

- Media Player
-  MPNowPlayingInfoPropertyPlaybackQueueIndex 

Global Variable

# MPNowPlayingInfoPropertyPlaybackQueueIndex

The index of the Now Playing item in the app’s playback queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.12.2+tvOSvisionOS 1.0+watchOS 5.0+

``` source
let MPNowPlayingInfoPropertyPlaybackQueueIndex: String
```

## Discussion

Value is an NSNumber object configured as an NSUInteger. The playback queue uses zero-based indexing. For example, to display first item in the queue as “item 1 of 10,” set the item’s index to `0`.

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

