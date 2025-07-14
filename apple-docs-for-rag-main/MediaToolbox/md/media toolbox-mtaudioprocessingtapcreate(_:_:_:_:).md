

- Media Toolbox
-  MTAudioProcessingTapCreate(\_:\_:\_:\_:) 

Function

# MTAudioProcessingTapCreate(\_:\_:\_:\_:)

Creates a new audio processing tap.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func MTAudioProcessingTapCreate(
    _ allocator: CFAllocator?,
    _ callbacks: UnsafePointer,
    _ flags: MTAudioProcessingTapCreationFlags,
    _ tapOut: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new tap. Pass `NULL` or `kCFAllocatorDefault` to use the current default allocator.

`callbacks`  

An callbacks struct. MTAudioProcessingTap makes a copy of this struct.

`flags`  

Flags that are used to control aspects of the processing tap. Valid flags are:

kMTAudioProcessingTapCreationFlag_PreEffects  
processing is done before any further effects are applied by the audio queue to the audio.

kMTAudioProcessingTapCreationFlag_PostEffects  
processing is done after all processing is done, including that of other taps.

`tapOut`  

The processing tap object.

## Return Value

An `OSStatus` result code.

## Overview

The processing tap will then be used to process decoded data. The processing is performed on audio either before or after any effects or other processing (varispeed, etc) is applied by the audio queue.

## Topics

### Flags

typealias MTAudioProcessingTapCreationFlags

Flags to use when creating audio processing taps.

### Callbacks

struct MTAudioProcessingTapCallbacks

A structure that defines life cycle callbacks for an audio processing tap object.

## See Also

### Audio Taps

func MTAudioProcessingTapGetSourceAudio(MTAudioProcessingTap, CMItemCount, UnsafeMutablePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;MTAudioProcessingTapFlags>?, UnsafeMutablePointer&lt;CMTimeRange>?, UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves source audio for an audio processing tap.

func MTAudioProcessingTapGetStorage(MTAudioProcessingTap) -> UnsafeMutableRawPointer

Retrieves a custom storage pointer for an audio processing tap.

func MTAudioProcessingTapGetTypeID() -> CFTypeID

Retrieves the type identifier for this audio processing tap.

typealias MTAudioProcessingTapFlags

Flags that indicate where to tap the audio.

class MTAudioProcessingTap

An audio processing tap object.

