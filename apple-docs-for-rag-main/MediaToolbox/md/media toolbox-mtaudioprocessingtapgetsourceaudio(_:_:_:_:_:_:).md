

- Media Toolbox
-  MTAudioProcessingTapGetSourceAudio(\_:\_:\_:\_:\_:\_:) 

Function

# MTAudioProcessingTapGetSourceAudio(\_:\_:\_:\_:\_:\_:)

Retrieves source audio for an audio processing tap.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func MTAudioProcessingTapGetSourceAudio(
    _ tap: MTAudioProcessingTap,
    _ numberFrames: CMItemCount,
    _ bufferListInOut: UnsafeMutablePointer,
    _ flagsOut: UnsafeMutablePointer?,
    _ timeRangeOut: UnsafeMutablePointer?,
    _ numberFramesOut: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`tap`  

The processing tap.

`numberFrames`  

The number of frames the processing tap requires for its processing.

`bufferListInOut`  

The audio buffer list which will contain the source data. On input, all fields except for the buffer pointers must be filled in. If the buffer pointers are NULL (recommended), non-NULL pointers will be returned and system owns the source buffers; these buffers are only applicable for the duration of the processing tap callback. If the buffer pointers are non-NULL, then they must be big enough to hold numberFrames, and the source data will be copied into these buffers.

`flagsOut`  

Flags to describe state about the input requested, e.g., discontinuity/complete. Can be NULL.

`timeRangeOut`  

The asset time range corresponding to the provided source audio frames. Can be NULL.

`numberFramesOut`  

The number of source frames that have been provided. Can be NULL. This can be less than the number of requested frames specified in numberFrames.

## Return Value

An `OSStatus` result code.

## Overview

This function may only be called from the processing tap’s callback.

## See Also

### Audio Taps

func MTAudioProcessingTapCreate(CFAllocator?, UnsafePointer&lt;MTAudioProcessingTapCallbacks>, MTAudioProcessingTapCreationFlags, UnsafeMutablePointer&lt;Unmanaged&lt;MTAudioProcessingTap>?>) -> OSStatus

Creates a new audio processing tap.

func MTAudioProcessingTapGetStorage(MTAudioProcessingTap) -> UnsafeMutableRawPointer

Retrieves a custom storage pointer for an audio processing tap.

func MTAudioProcessingTapGetTypeID() -> CFTypeID

Retrieves the type identifier for this audio processing tap.

typealias MTAudioProcessingTapFlags

Flags that indicate where to tap the audio.

class MTAudioProcessingTap

An audio processing tap object.

