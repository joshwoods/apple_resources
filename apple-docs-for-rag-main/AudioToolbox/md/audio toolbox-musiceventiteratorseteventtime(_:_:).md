

- Audio Toolbox
-  MusicEventIteratorSetEventTime(\_:\_:) 

Function

# MusicEventIteratorSetEventTime(\_:\_:)

Sets the timestamp for the event at a music event iterator’s current position.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func MusicEventIteratorSetEventTime(
    _ inIterator: MusicEventIterator,
    _ inTimeStamp: MusicTimeStamp
) -> OSStatus
```

## Parameters 

`inIterator`  

The music event iterator whose current event you want to change the timestamp of.

`inTimeStamp`  

The new timestamp for the event, in beats.

## Return Value

A result code.

## Discussion

After calling this function, the music event iterator remains positioned at the same event. However, because the event has been moved to a new location on the iterator’s music track, the iterator may no longer have a next or previous event. You can test this by calling MusicEventIteratorHasPreviousEvent(_:_:) and MusicEventIteratorHasNextEvent(_:_:).

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

typealias MusicEventIterator

A music event iterator sequentially handles events on a music track.

typealias MusicEventType

MIDI and other music event types, used by music event iterator functions.

struct ExtendedNoteOnEvent

Describes a note-on event with extended parameters.

struct ExtendedTempoEvent

Describes a music track tempo in beats-per-minute.

