

- Audio Toolbox
-  MusicEventType 

Type Alias

# MusicEventType

MIDI and other music event types, used by music event iterator functions.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MusicEventType = UInt32
```

## Topics

### Constants

var kMusicEventType_NULL: UInt32

A null music event.

var kMusicEventType_ExtendedNote: UInt32

A non-MIDI music event with variable number of parameters.

var kMusicEventType_ExtendedTempo: UInt32

An event that signals a change in tempo, in beats-per-minute.

var kMusicEventType_User: UInt32

User-defined data.

var kMusicEventType_Meta: UInt32

A standard MIDI file metaevent.

var kMusicEventType_MIDINoteMessage: UInt32

A MIDI note-on message, including duration.

var kMusicEventType_MIDIChannelMessage: UInt32

A MIDI channel message, other than note control.

var kMusicEventType_MIDIRawData: UInt32

MIDI system-exclusive data.

var kMusicEventType_Parameter: UInt32

An audio unit parameter event.

var kMusicEventType_AUPreset: UInt32

An event containing an audio unit user preset dictionary.

## See Also

### Iterating Over Music Events

func NewMusicEventIterator(MusicTrack, UnsafeMutablePointer&lt;MusicEventIterator?>) -> OSStatus

Creates a new music event iterator.

func DisposeMusicEventIterator(MusicEventIterator) -> OSStatus

Disposes of a music event iterator.

func MusicEventIteratorNextEvent(MusicEventIterator) -> OSStatus

Positions a music event iterator at the next event on a music track.

func MusicEventIteratorSeek(MusicEventIterator, MusicTimeStamp) -> OSStatus

Positions a music event iterator at a specified timestamp, in beats.

func MusicEventIteratorDeleteEvent(MusicEventIterator) -> OSStatus

Deletes the event at a music event iterator’s current position.

func MusicEventIteratorGetEventInfo(MusicEventIterator, UnsafeMutablePointer&lt;MusicTimeStamp>, UnsafeMutablePointer&lt;MusicEventType>, UnsafeMutablePointer&lt;UnsafeRawPointer?>, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets information about the event at a music event iterator’s current position.

func MusicEventIteratorHasCurrentEvent(MusicEventIterator, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates whether or not a music track contains an event at the music event iterator’s current position.

func MusicEventIteratorHasNextEvent(MusicEventIterator, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates whether or not a music track contains an event beyond the music event iterator’s current position.

func MusicEventIteratorHasPreviousEvent(MusicEventIterator, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates whether or not a music track contains an event before the music event iterator’s current position.

func MusicEventIteratorPreviousEvent(MusicEventIterator) -> OSStatus

Positions a music event iterator at the previous event on a music track.

func MusicEventIteratorSetEventInfo(MusicEventIterator, MusicEventType, UnsafeRawPointer) -> OSStatus

Sets information for the event at a music event iterator’s current position.

func MusicEventIteratorSetEventTime(MusicEventIterator, MusicTimeStamp) -> OSStatus

Sets the timestamp for the event at a music event iterator’s current position.

typealias MusicEventIterator

A music event iterator sequentially handles events on a music track.

struct ExtendedNoteOnEvent

Describes a note-on event with extended parameters.

struct ExtendedTempoEvent

Describes a music track tempo in beats-per-minute.

