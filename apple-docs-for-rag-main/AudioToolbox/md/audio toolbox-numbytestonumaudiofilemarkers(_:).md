

- Audio Toolbox
-  NumBytesToNumAudioFileMarkers(\_:) 

Function

# NumBytesToNumAudioFileMarkers(\_:)

A macro that returns the number of audio file markers represented by a specified number of bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func NumBytesToNumAudioFileMarkers(_ inNumBytes: Int) -> Int
```

## Parameters 

`inNumBytes`  

The number of bytes for which you wish to know the equivalent number of audio file markers.

## Return Value

The number of audio file markers that can be contained in the specified number of bytes.

## Discussion

Use this convenience macro when you call the AudioFileGetProperty(_:_:_:_:) function with the kAudioFilePropertyMarkerList property to calculate the number of markers that will be returned.

## See Also

### Related Documentation

func AudioFileGetProperty(AudioFileID, AudioFilePropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets the value of an audio file property.

### Parsing Audio File Content

func NextAudioFileRegion(UnsafePointer&lt;AudioFileRegion>) -> UnsafeMutablePointer&lt;AudioFileRegion>

Finds the next audio file region in a region list.

func NumAudioFileMarkersToNumBytes(Int) -> Int

Returns the number of bytes corresponding to a specified number of audio file markers.

