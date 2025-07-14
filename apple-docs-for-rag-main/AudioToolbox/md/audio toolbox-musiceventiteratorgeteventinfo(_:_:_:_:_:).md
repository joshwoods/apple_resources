

- Audio Toolbox
-  MusicEventIteratorGetEventInfo(\_:\_:\_:\_:\_:) 

Function

# MusicEventIteratorGetEventInfo(\_:\_:\_:\_:\_:)

Gets information about the event at a music event iterator’s current position.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func MusicEventIteratorGetEventInfo(
    _ inIterator: MusicEventIterator,
    _ outTimeStamp: UnsafeMutablePointer,
    _ outEventType: UnsafeMutablePointer,
    _ outEventData: UnsafeMutablePointer,
    _ outEventDataSize: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inIterator`  

The music event iterator whose current event you want information about.

`outTimeStamp`  

On output, the timestamp of the music event, in beats.

`outEventType`  

On output, the type of music event. For possible event types, see MusicEventType.

`outEventData`  

On output, a reference to the music event data. The type of data is specified by the `outEventType` parameter. Do not modify the referenced data directly; to change an event, use the MusicEventIteratorSetEventInfo(_:_:_:) function.

`outEventDataSize`  

On output, the size, in bytes, of the music event data in the `outEventData` parameter.

## Return Value

A result code.

## Discussion

Pass `NULL` for any output parameter whose information you do not need.

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

typealias MusicEventType

MIDI and other music event types, used by music event iterator functions.

struct ExtendedNoteOnEvent

Describes a note-on event with extended parameters.

struct ExtendedTempoEvent

Describes a music track tempo in beats-per-minute.

