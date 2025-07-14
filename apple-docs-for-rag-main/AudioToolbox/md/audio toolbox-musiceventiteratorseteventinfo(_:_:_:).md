

- Audio Toolbox
-  MusicEventIteratorSetEventInfo(\_:\_:\_:) 

Function

# MusicEventIteratorSetEventInfo(\_:\_:\_:)

Sets information for the event at a music event iterator’s current position.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func MusicEventIteratorSetEventInfo(
    _ inIterator: MusicEventIterator,
    _ inEventType: MusicEventType,
    _ inEventData: UnsafeRawPointer
) -> OSStatus
```

## Parameters 

`inIterator`  

The music event iterator whose current event you want to set.

`inEventType`  

The type of music event that you are specifying. For possible event types, see MusicEventType.

`inEventData`  

The event data that you are specifying. The size and type of the data must be appropriate for the music event type you specify in the `inEventType` parameter.

## Return Value

A result code.

## Discussion

Use this function to set the music event type and event data for the event that a music event iterator is positioned at. This function doesn’t allow you to change an event’s timestamp; to do that, call the MusicEventIteratorSetEventTime(_:_:) function.

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

func MusicEventIteratorSetEventTime(MusicEventIterator, MusicTimeStamp) -> OSStatus

Sets the timestamp for the event at a music event iterator’s current position.

typealias MusicEventIterator

A music event iterator sequentially handles events on a music track.

typealias MusicEventType

MIDI and other music event types, used by music event iterator functions.

struct ExtendedNoteOnEvent

Describes a note-on event with extended parameters.

struct ExtendedTempoEvent

Describes a music track tempo in beats-per-minute.

