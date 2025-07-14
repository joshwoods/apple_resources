

- Audio Toolbox
-  NextAudioFileRegion(\_:) 

Function

# NextAudioFileRegion(\_:)

Finds the next audio file region in a region list.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func NextAudioFileRegion(_ inAFRegionPtr: UnsafePointer) -> UnsafeMutablePointer
```

## Parameters 

`inAFRegionPtr`  

A pointer to an audio file region in the region list.

## Return Value

A pointer to the next region after the region pointed to by the `inAFRegionPtr` parameter. This value can be beyond the end of the list, so pay attention to the total number of regions in the list.

## Discussion

Because audio file regions are of variable length, you cannot easily walk the list. Use this convenience function when you call the AudioFileGetProperty(_:_:_:_:) function with the kAudioFilePropertyRegionList property to walk through the list of regions returned.

## See Also

### Related Documentation

func AudioFileSetProperty(AudioFileID, AudioFilePropertyID, UInt32, UnsafeRawPointer) -> OSStatus

Sets the value of an audio file property

### Parsing Audio File Content

func NumAudioFileMarkersToNumBytes(Int) -> Int

Returns the number of bytes corresponding to a specified number of audio file markers.

func NumBytesToNumAudioFileMarkers(Int) -> Int

A macro that returns the number of audio file markers represented by a specified number of bytes.

