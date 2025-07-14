

- AVFAudio
-  AVMusicEventEnumerationBlock 

Type Alias

# AVMusicEventEnumerationBlock

A type you use to enumerate and remove music events, if necessary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias AVMusicEventEnumerationBlock = (AVMusicEvent, UnsafeMutablePointer, UnsafeMutablePointer) -> Void
```

## Parameters 

`event`  

The music event the block returns.

`timeStamp`  

The beat position of the event in the music track.

`removeEvent`  

A value that determines whether to remove the event from the track.

## Discussion

You use this type when you use enumerateEvents(in:using:). If you modify `event` or `timeStamp`, you change the corresponding value in the track event.

## See Also

### Iterating Over Events

func enumerateEvents(in: AVBeatRange, using: (AVMusicEvent, UnsafeMutablePointer&lt;AVMusicTimeStamp>, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Iterates through the music events within the track.

