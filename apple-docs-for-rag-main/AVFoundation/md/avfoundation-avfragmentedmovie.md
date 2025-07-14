

- AVFoundation
-  AVFragmentedMovie 

Class

# AVFragmentedMovie

An object that represents a fragmented movie file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
class AVFragmentedMovie
```

## Topics

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVFragmentedMovieTrack]>

The tracks that a movie contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVFragmentedMovieTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVFragmentedMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVFragmentedMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

### Accessing Tracks

Prefer loading tracks asynchronously using the methods in Loading Tracks.

var tracks: [AVFragmentedMovieTrack]

The tracks that a movie contains.

func track(withTrackID: CMPersistentTrackID) -> AVFragmentedMovieTrack?

Retrieves a track in the movie that contains the specified identifier.

Deprecated

func tracks(withMediaType: AVMediaType) -> [AVFragmentedMovieTrack]

Retrieves tracks in the movie that present media of the specified type.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVFragmentedMovieTrack]

Retrieves tracks in the movie that present media of the specified characteristic.

Deprecated

## Relationships

### Inherits From

- AVMovie

### Conforms To

- AVAsynchronousKeyValueLoading
- AVFragmentMinding
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- Sendable

## See Also

### Fragmented movies

class AVFragmentedMovieTrack

An object that represents a track in a fragmented movie.

class AVFragmentedMovieMinder

An object that checks whether a fragmented movie appends additional movie fragments.

protocol AVFragmentMinding

A protocol that defines whether an asset supports fragment minding.

