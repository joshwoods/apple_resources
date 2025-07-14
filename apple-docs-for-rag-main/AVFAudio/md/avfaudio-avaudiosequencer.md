

- AVFAudio
-  AVAudioSequencer 

Class

# AVAudioSequencer

An object that plays audio from a collection of MIDI events the system organizes into music tracks.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioSequencer
```

## Topics

### Creating an Audio Sequencer

init()

Creates an audio sequencer object.

init(audioEngine: AVAudioEngine)

Creates an audio sequencer that the framework attaches to an audio engine instance.

### Writing to a MIDI File

func write(to: URL, smpteResolution: Int, replaceExisting: Bool) throws

Creates and writes a MIDI file from the events in the sequence.

### Handling Music Tracks

class AVMusicTrack

A collection of music events that you can offset, set to a muted state, modify independently from other track events, and send to a specified destination.

func createAndAppendTrack() -> AVMusicTrack

Creates a new music track and appends it to the sequencer’s list.

func reverseEvents()

Reverses the order of all events in all music tracks, including the tempo track.

func removeTrack(AVMusicTrack) -> Bool

Removes the music track from the sequencer.

enum AVMusicTrackLoopCount

Options that define the number of times a track loops.

### Handling Music Events

class AVMusicEvent

A base class for the events you associate with a music track.

class AVMusicUserEvent

An object that represents a custom user message.

class AVParameterEvent

An object that represents a parameter event on a music track’s destination.

class AVAUPresetEvent

An object that represents a preset load and change on the music track’s destination audio unit.

class AVExtendedTempoEvent

An object that represents a tempo change to a specific beats-per-minute value.

class AVExtendedNoteOnEvent

An object that represents a custom extension of a MIDI note on event.

### Handling MIDI Events

class AVMIDINoteEvent

An object that represents MIDI note on or off messages.

class AVMIDIMetaEvent

An object that represents MIDI meta event messages.

class AVMIDISysexEvent

An object that represents a MIDI system exclusive message.

### Handling MIDI Channel Events

class AVMIDIChannelEvent

A base class for all MIDI messages that operate on a single MIDI channel.

class AVMIDIChannelPressureEvent

An object that represents a MIDI channel pressure message.

class AVMIDIProgramChangeEvent

An object that represents a MIDI program or patch change message.

class AVMIDIPolyPressureEvent

An object that represents a MIDI poly or key pressure event.

class AVMIDIPitchBendEvent

An object that represents a MIDI pitch bend message.

class AVMIDIControlChangeEvent

An object that represents a MIDI control change message.

### Managing Sequence Load Options

func load(from: Data, options: AVMusicSequenceLoadOptions) throws

Parses the data and adds its events to the sequence.

func load(from: URL, options: AVMusicSequenceLoadOptions) throws

Loads the file the URL references and adds the events to the sequence.

struct AVMusicSequenceLoadOptions

A structure that defines whether data on different MIDI channels map to multiple tracks, or whether the framework preserves the tracks as they are.

### Operating an Audio Sequencer

func prepareToPlay()

Gets ready to play the sequence by prerolling all events.

func start() throws

Starts the sequencer’s player.

func stop()

Stops the sequencer’s player.

### Managing Time Stamps

typealias AVMusicTimeStamp

A fractional number of beats.

func hostTime(forBeats: AVMusicTimeStamp, error: NSErrorPointer) -> UInt64

Gets the host time the sequence plays at the specified position.

func seconds(forBeats: AVMusicTimeStamp) -> TimeInterval

Gets the time for the specified beat position (timestamp) in the track, in seconds.

### Handling Beat Range

func beats(forHostTime: UInt64, error: NSErrorPointer) -> AVMusicTimeStamp

Gets the beat the system plays at the specified host time.

func beats(forSeconds: TimeInterval) -> AVMusicTimeStamp

Gets the beat position (timestamp) for the specified time in the track.

var AVMusicTimeStampEndOfTrack: Double

A timestamp you use to access all events in a music track through a beat range.

typealias AVBeatRange

A specific time range within a music track.

### Setting the User Callback

func setUserCallback(AVAudioSequencerUserCallback?)

Adds a callback that the sequencer calls each time it encounters a user event during playback.

typealias AVAudioSequencerUserCallback

A callback the sequencer calls asynchronously during playback when it encounters a user event.

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

struct InfoDictionaryKey

Constants that defines metadata keys for a sequencer.

func data(withSMPTEResolution: Int, error: NSErrorPointer) -> Data

Gets a data object that contains the events from the sequence.

var AVMusicTimeStampEndOfTrack: Double

A timestamp you use to access all events in a music track through a beat range.

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

### MIDI

class AVAudioUnitSampler

An object that you configure with one or more instrument samples, based on Apple’s Sampler audio unit.

