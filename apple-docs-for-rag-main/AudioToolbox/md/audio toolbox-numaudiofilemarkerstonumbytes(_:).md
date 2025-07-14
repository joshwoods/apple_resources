

- Audio Toolbox
-  NumAudioFileMarkersToNumBytes(\_:) 

Function

# NumAudioFileMarkersToNumBytes(\_:)

Returns the number of bytes corresponding to a specified number of audio file markers.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func NumAudioFileMarkersToNumBytes(_ inNumMarkers: Int) -> Int
```

## Parameters 

`inNumMarkers`  

The number of audio file markers for which you wish to know the equivalent number of bytes.

## Return Value

The number of bytes required to contain the specified number of audio file markers.

## Discussion

Use this convenience function when you call the AudioFileSetProperty(_:_:_:_:) function with the kAudioFilePropertyMarkerList property to calculate the size of buffer needed to hold a specific number of audio file markers.

## See Also

### Related Documentation

func AudioFileSetProperty(AudioFileID, AudioFilePropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of an audio file property

### Parsing Audio File Content

func NextAudioFileRegion(UnsafePointer&lt;AudioFileRegion>) -> UnsafeMutablePointer&lt;AudioFileRegion>

Finds the next audio file region in a region list.

func NumBytesToNumAudioFileMarkers(Int) -> Int

A macro that returns the number of audio file markers represented by a specified number of bytes.

