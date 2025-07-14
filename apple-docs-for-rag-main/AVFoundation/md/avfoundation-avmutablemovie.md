

- AVFoundation
-  AVMutableMovie 

Class

# AVMutableMovie

A mutable object that represents an audiovisual container that conforms to the QuickTime movie file format or a related format like MPEG-4.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
class AVMutableMovie
```

## Overview

This class is a mutable subclass of AVMovie that provides methods that support movie editing. For example, you can use a mutable movie to copy media data from one track and paste it into another. You can also use this object to create track references from one track to another (for example, to set one track as a chapter track of another track). To perform editing operations on individual tracks, use the associated classes AVMovieTrack and AVMutableMovieTrack.

You use movie objects only when operating on format-specific features of a QuickTime or ISO base media file. You typically don’t use these classes to open and play QuickTime movie files or ISO base media files. Instead, you use AVURLAsset and AVPlayerItem.

When performing media insertions, a movie interleaves media data from tracks in the source asset to optimize the movie file for playback. However, performing a series of media insertions may result in a movie file that’s not optimally interleaved. You can optimize a movie file for playback by exporting it with an AVAssetExportSession object using the export preset AVAssetExportPresetPassthrough, and setting the shouldOptimizeForNetworkUse property value to true.

## Topics

### Creating a Movie

init(url: URL, options: [String : Any]?, error: ()) throws

Creates a mutable movie object from a movie header stored in a QuickTime movie file of ISO base media file.

init(data: Data, options: [String : Any]?, error: ()) throws

Creates a mutable movie object from a movie stored in a data object.

init(settingsFrom: AVMovie?, options: [String : Any]?) throws

Creates a mutable movie object without tracks.

### Configuring a Movie

var isModified: Bool

A Boolean value that indicates whether the movie is in a modified state.

var timescale: CMTimeScale

The time scale of the movie.

var interleavingPeriod: CMTime

A time period indicating the duration for interleaving runs of samples for each track.

var defaultMediaDataStorage: AVMediaDataStorage?

The default storage container for media data that you add to a movie.

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVMutableMovieTrack]>

The tracks that a movie contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVMutableMovieTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVMutableMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVMutableMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

### Accessing Tracks

Prefer loading tracks asynchronously using the methods in Loading Tracks.

var tracks: [AVMutableMovieTrack]

The tracks that a movie contains.

func track(withTrackID: CMPersistentTrackID) -> AVMutableMovieTrack?

Retrieves a track in the movie that contains the specified identifier.

func tracks(withMediaType: AVMediaType) -> [AVMutableMovieTrack]

Retrieves tracks in the movie that present media of the specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMutableMovieTrack]

Retrieve tracks in the movie that present media of the specified characteristic.

func unusedTrackID() -> CMPersistentTrackID

Returns an identifier that no other tracks in the asset use.

### Accessing Track Groups

var trackGroups: [AVAssetTrackGroup]

The track groups an asset contains.

### Managing Tracks

func mutableTrack(compatibleWith: AVAssetTrack) -> AVMutableMovieTrack?

Provides a reference to a track from a mutable movie into which you can insert any time range.

func addMutableTrack(withMediaType: AVMediaType, copySettingsFrom: AVAssetTrack?, options: [String : Any]?) -> AVMutableMovieTrack?

Adds an empty track to the target movie.

func addMutableTracksCopyingSettings(from: [AVAssetTrack], options: [String : Any]?) -> [AVMutableMovieTrack]

Adds one or more empty tracks to the target movie and copies the track settings from the source tracks.

func removeTrack(AVMovieTrack)

Removes the specified track from the target movie.

### Managing Time Ranges

func insertEmptyTimeRange(CMTimeRange)

Adds an empty time range to a movie.

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime, copySampleData: Bool) throws

Inserts all of the tracks in a specified time range of an asset into a movie.

func scale(CMTimeRange, toDuration: CMTime)

Changes the duration of a time range in a movie.

func removeTimeRange(CMTimeRange)

Removes the specified time range from a movie.

### Accessing Duration and Timing

var duration: CMTime

A time value that indicates the asset’s duration.

var providesPreciseDurationAndTiming: Bool

A Boolean value that indicates whether the asset provides precise duration and timing.

var minimumTimeOffsetFromLive: CMTime

A time value that indicates how closely playback follows the latest live stream content.

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers for which a value is available.

var commonMetadata: [AVMetadataItem]

The metadata items an asset contains for common metadata identifiers that provide a value.

var availableMetadataFormats: [AVMetadataFormat]

The metadata formats this asset contains.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns an array of metadata items from the container with the specified format.

var creationDate: AVMetadataItem?

A metadata item that indicates the asset’s creation date.

var lyrics: String?

The lyrics of the asset in a language suitable for the current locale.

### Determining Suitability

var isPlayable: Bool

A Boolean value that indicates whether the asset has playable content.

var isReadable: Bool

A Boolean value that indicates whether you can extract the asset’s media data using an asset reader.

var isExportable: Bool

A Boolean value that indicates whether you can export this asset using an export session.

var isComposable: Bool

A Boolean value that indicates whether you can use the asset as a segment of a composition track.

var isCompatibleWithAirPlayVideo: Bool

A Boolean value that indicates whether the asset is compatible with AirPlay Video.

var isCompatibleWithSavedPhotosAlbum: Bool

A Boolean value that indicates whether you can write the composition to the Saved Photos album.

### Inspecting Preferences

var preferredRate: Float

The asset’s rate preference for playing its media.

var preferredVolume: Float

The asset’s volume preference for playing its audible media.

var preferredTransform: CGAffineTransform

The asset’s transform preference to apply to its visual content during presentation or processing.

var preferredMediaSelection: AVMediaSelection

The default media selections for this asset’s media selection groups.

### Accessing Media Selections

var allMediaSelections: [AVMediaSelection]

The array of available media selections for this asset.

var availableMediaCharacteristicsWithMediaSelectionOptions: [AVMediaCharacteristic]

An array of media characteristics for which a media selection option is available.

func mediaSelectionGroup(forMediaCharacteristic: AVMediaCharacteristic) -> AVMediaSelectionGroup?

Returns a media selection group that contains one or more options with the specified media characteristic.

### Accessing Chapter Metadata

var availableChapterLocales: [Locale]

The locales of the asset’s chapter metadata.

func chapterMetadataGroups(bestMatchingPreferredLanguages: [String]) -> [AVTimedMetadataGroup]

Returns an array of chapters with a locale that best matches the list of preferred languages.

func chapterMetadataGroups(withTitleLocale: Locale, containingItemsWithCommonKeys: [AVMetadataKey]?) -> [AVTimedMetadataGroup]

Returns an array of chapters that contain the specified title locale and common keys.

### Determining Content Protections

var hasProtectedContent: Bool

A Boolean value that indicates whether the asset contains protected content.

### Determining Fragment Support

var canContainFragments: Bool

A Boolean value that indicates whether you can extend the asset by fragments.

var containsFragments: Bool

A Boolean value that indicates whether at least one movie fragment extends the asset.

var overallDurationHint: CMTime

The total duration of fragments that currently exist, or may exist in the future.

## Relationships

### Inherits From

- AVMovie

### Conforms To

- AVAsynchronousKeyValueLoading
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Mutable movies

class AVMutableMovieTrack

A mutable track that conforms to the QuickTime or ISO base media file format.

