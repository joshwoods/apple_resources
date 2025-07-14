

- AVFAudio
- AVMusicTrack
-  enumerateEvents(in:using:) 

Instance Method

# enumerateEvents(in:using:)

Iterates through the music events within the track.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func enumerateEvents(
    in range: AVBeatRange,
    using block: (AVMusicEvent, UnsafeMutablePointer, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`range`  

The range to iterate through.

`block`  

The block to call for each event.

## Discussion

Examine each event the block returns by using isKind(of:) to determine the subclass, and then cast and access it accordingly.

The iteration may continue after removing an event.

The event object returned through the block won’t be the same instances you add to the AVMusicTrack, though the content is identical.

## See Also

### Iterating Over Events

typealias AVMusicEventEnumerationBlock

A type you use to enumerate and remove music events, if necessary.

