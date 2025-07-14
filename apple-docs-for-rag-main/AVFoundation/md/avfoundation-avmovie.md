

- AVFoundation
-  AVMovie 

Class

# AVMovie

An object that represents an audiovisual container that conforms to the QuickTime movie file format or a related format like MPEG-4.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
class AVMovie
```

## Overview

`AVMovie` supports operations involving the format-specific portions of the QuickTime movie model that AVAsset doesn’t support. For instance, retrieving the movie header from an existing QuickTime movie file. You can also use `AVMovie` to write a movie header into a new file, thereby creating a reference movie.

## Topics

### Creating a Movie

convenience init(url: URL)

Creates a movie that models the media at the specified URL.

init(url: URL, options: [String : Any]?)

Creates a movie object from a movie header stored in a QuickTime movie file of ISO base media file.

init(data: Data, options: [String : Any]?)

Creates a movie object from a movie file’s data.

Initialization Options

Specify options to configure the initialization of a movie.

### Determining Supported File Types

class func movieTypes() -> [AVFileType]

Returns the file types that a movie supports.

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVMovieTrack]>

The tracks that a movie contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVMovieTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

### Creating and Writing Headers

func `is`(compatibleWithFileType: AVFileType) -> Bool

Returns a Boolean value that indicates whether the system can create a movie header of the specified type.

func makeMovieHeader(fileType: AVFileType) throws -> Data

Creates a header for a movie for the specified file type.

func writeHeader(to: URL, fileType: AVFileType, options: AVMovieWritingOptions) throws

Writes the movie header to the specified URL.

struct AVMovieWritingOptions

A structure that defines options to control the writing of a movie header to a destination URL.

### Determining Fragment Support

var canContainMovieFragments: Bool

A Boolean value that indicates whether fragments can extend the movie file.

var containsMovieFragments: Bool

A Boolean value that indicates whether at least one movie fragment extends the movie file.

### Accessing Movie Information

var url: URL?

A URL to a QuickTime or ISO base media file.

var data: Data?

A data object that contains the movie file’s data.

### Accessing Tracks

Prefer loading tracks asynchronously using the methods in Loading Tracks.

var tracks: [AVMovieTrack]

The tracks that a movie contains.

func track(withTrackID: CMPersistentTrackID) -> AVMovieTrack?

Retrieves a track in the movie that contains the specified identifier.

Deprecated

func tracks(withMediaType: AVMediaType) -> [AVMovieTrack]

Retrieves tracks in the movie that present media of the specified type.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMovieTrack]

Retrieves tracks in the movie that present media of the specified characteristic.

Deprecated

### Accessing Data Storage

var defaultMediaDataStorage: AVMediaDataStorage?

The default storage container for media data added to a movie.

## Relationships

### Inherits From

- AVAsset

### Inherited By

- AVFragmentedMovie
- AVMutableMovie

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

### Movies

class AVMovieTrack

A track in a movie that conforms to the QuickTime or ISO base media file format.

