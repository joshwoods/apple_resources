

- Audio Toolbox
-  MusicEventIteratorNextEvent(\_:) 

Function

# MusicEventIteratorNextEvent(\_:)

Positions a music event iterator at the next event on a music track.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func MusicEventIteratorNextEvent(_ inIterator: MusicEventIterator) -> OSStatus
```

## Parameters 

`inIterator`  

The music event iterator to reposition.

## Return Value

A result code.

## Discussion

Use this function to increment the position of a music event iterator forward through a music track’s events.

If an iterator is at the final event of a track when you call this function, the iterator then moves beyond the final event. You can detect if the iterator is beyond the final event by calling the MusicEventIteratorHasCurrentEvent(_:_:) function.

The following code snippet illustrates how to use a music event iterator to proceed forward along a music track, from the start:

```
// Create a new iterator, which automatically points at the first event
// on the iterator's music track.

bool hasCurrentEvent;
MusicEventIteratorHasCurrentEvent (myIterator, &hasCurrentEvent);
while (hasCurrentEvent) {
        // do work here
    MusicEventIteratorNextEvent (myIterator);
    MusicEventIteratorHasCurrentEvent (myIterator, &hasCurrentEvent);
}
```

## See Also

### Iterating Over Music Events

func NewMusicEventIterator(MusicTrack, UnsafeMutablePointer&lt;MusicEventIterator?>) -> OSStatus

Creates a new music event iterator.

func DisposeMusicEventIterator(MusicEventIterator) -> OSStatus

Disposes of a music event iterator.

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

typealias MusicEventType

MIDI and other music event types, used by music event iterator functions.

struct ExtendedNoteOnEvent

Describes a note-on event with extended parameters.

struct ExtendedTempoEvent

Describes a music track tempo in beats-per-minute.

