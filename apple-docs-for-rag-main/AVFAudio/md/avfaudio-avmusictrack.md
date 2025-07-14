

- AVFAudio
-  AVMusicTrack 

Class

# AVMusicTrack

A collection of music events that you can offset, set to a muted state, modify independently from other track events, and send to a specified destination.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class AVMusicTrack
```

## Topics

### Configuring Music Track Properties

var isMuted: Bool

A Boolean value that indicates whether the track is in a muted state.

var isSoloed: Bool

A Boolean value that indicates whether the track is in a soloed state.

var offsetTime: AVMusicTimeStamp

The offset of the track’s start time, in beats.

var timeResolution: Int

The time resolution value for the sequence, in ticks (pulses) per quarter note.

var usesAutomatedParameters: Bool

A Boolean value that indicates whether the track is an automation track.

### Configuring the Track Duration

var lengthInBeats: AVMusicTimeStamp

The total duration of the track, in beats.

var lengthInSeconds: TimeInterval

The total duration of the track, in seconds.

### Configuring the Track Destinations

var destinationAudioUnit: AVAudioUnit?

The audio unit that receives the track’s events.

var destinationMIDIEndpoint: MIDIEndpointRef

The MIDI endpoint you specify as the track’s target.

### Configuring the Looping State

var isLoopingEnabled: Bool

A Boolean value that indicates whether the track is in a looping state.

var loopRange: AVBeatRange

The timestamp range for the loop, in beats.

var numberOfLoops: Int

The number of times the track’s loop repeats.

### Adding and Clearing Events

func addEvent(AVMusicEvent, at: AVMusicTimeStamp)

Adds a music event to a track at the time you specify.

func moveEvents(in: AVBeatRange, by: AVMusicTimeStamp)

Moves the beat location of all events in the given beat range by the amount you specify.

func clearEvents(in: AVBeatRange)

Removes all events in the given beat range from the music track.

### Cutting and Copying Events

func cutEvents(in: AVBeatRange)

Splices all events in the beat range from the music track.

func copyEvents(in: AVBeatRange, from: AVMusicTrack, insertAt: AVMusicTimeStamp)

Copies the events from the source track and splices them into the current music track.

func copyAndMergeEvents(in: AVBeatRange, from: AVMusicTrack, mergeAt: AVMusicTimeStamp)

Copies the events from the source track and merges them into the current music track.

### Iterating Over Events

func enumerateEvents(in: AVBeatRange, using: (AVMusicEvent, UnsafeMutablePointer&lt;AVMusicTimeStamp>, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Iterates through the music events within the track.

typealias AVMusicEventEnumerationBlock

A type you use to enumerate and remove music events, if necessary.

### Getting the End of Track Timestamp

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

### Handling Music Tracks

func createAndAppendTrack() -> AVMusicTrack

Creates a new music track and appends it to the sequencer’s list.

func reverseEvents()

Reverses the order of all events in all music tracks, including the tempo track.

func removeTrack(AVMusicTrack) -> Bool

Removes the music track from the sequencer.

enum AVMusicTrackLoopCount

Options that define the number of times a track loops.

