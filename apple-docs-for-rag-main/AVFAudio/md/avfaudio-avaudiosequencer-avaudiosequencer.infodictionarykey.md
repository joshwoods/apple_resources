

- AVFAudio
- AVAudioSequencer
-  AVAudioSequencer.InfoDictionaryKey 

Structure

# AVAudioSequencer.InfoDictionaryKey

Constants that defines metadata keys for a sequencer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct InfoDictionaryKey
```

## Topics

### Getting Album Details

static let album: AVAudioSequencer.InfoDictionaryKey

A key that represents the album.

static let artist: AVAudioSequencer.InfoDictionaryKey

A key that represents the artist.

static let comments: AVAudioSequencer.InfoDictionaryKey

A key that represents the comments.

static let composer: AVAudioSequencer.InfoDictionaryKey

A key that represents the composer.

static let copyright: AVAudioSequencer.InfoDictionaryKey

A key that represents the copyright statement.

static let genre: AVAudioSequencer.InfoDictionaryKey

A key that represents the genre.

static let lyricist: AVAudioSequencer.InfoDictionaryKey

A key that represents the lyricist.

static let title: AVAudioSequencer.InfoDictionaryKey

A key that represents the title.

static let trackNumber: AVAudioSequencer.InfoDictionaryKey

A key that represents the track number.

static let subTitle: AVAudioSequencer.InfoDictionaryKey

A key that represents the subtitle.

static let year: AVAudioSequencer.InfoDictionaryKey

A key that represents the year.

### Getting the Duration and Time

static let approximateDurationInSeconds: AVAudioSequencer.InfoDictionaryKey

A key that represents the approximate duration.

static let timeSignature: AVAudioSequencer.InfoDictionaryKey

A key that represents the time signature.

static let tempo: AVAudioSequencer.InfoDictionaryKey

A key that represents the tempo.

### Getting the Recording Date

static let recordedDate: AVAudioSequencer.InfoDictionaryKey

A key that represents the date of the recording.

### Getting Encoding Information

static let encodingApplication: AVAudioSequencer.InfoDictionaryKey

A key that represents the encoding application.

static let sourceEncoder: AVAudioSequencer.InfoDictionaryKey

A key that represents the encoder the source uses.

static let nominalBitRate: AVAudioSequencer.InfoDictionaryKey

A key that represents the nominal bit rate.

static let sourceBitDepth: AVAudioSequencer.InfoDictionaryKey

A key that represents the bit depth of the source.

static let keySignature: AVAudioSequencer.InfoDictionaryKey

A key that represents the key signature.

### Getting the Channel Layout

static let channelLayout: AVAudioSequencer.InfoDictionaryKey

A key that represents the channel layout.

### Getting the Recording Code

static let ISRC: AVAudioSequencer.InfoDictionaryKey

A key that represents the international standard recording code.

### Creating a Dictionary Key

init(rawValue: String)

Creates a new instance with the raw value you specify.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Sequence Properties

var isPlaying: Bool

A Boolean value that indicates whether the sequencer’s player is in a playing state.

var rate: Float

The playback rate of the sequencer’s player.

var tracks: [AVMusicTrack]

An array that contains all the tracks in the sequence.

var currentPositionInBeats: TimeInterval

The current playback position, in beats.

var currentPositionInSeconds: TimeInterval

The current playback position, in seconds.

var tempoTrack: AVMusicTrack

The track that contains tempo information about the sequence.

var userInfo: [String : Any]

A dictionary that contains metadata from a sequence.

func data(withSMPTEResolution: Int, error: NSErrorPointer) -> Data

Gets a data object that contains the events from the sequence.

var AVMusicTimeStampEndOfTrack: Double

A timestamp you use to access all events in a music track through a beat range.

