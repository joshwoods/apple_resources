

- Media Toolbox
-  MTAudioProcessingTapFlags 

Type Alias

# MTAudioProcessingTapFlags

Flags that indicate where to tap the audio.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
typealias MTAudioProcessingTapFlags = UInt32
```

## Topics

### Flags

var kMTAudioProcessingTapFlag_EndOfStream: MTAudioProcessingTapFlags

Signifies that the source audio is past the end of stream.

var kMTAudioProcessingTapFlag_StartOfStream: MTAudioProcessingTapFlags

Signifies that the source audio is the beginning of a continuous stream.

## See Also

### Audio Taps

func MTAudioProcessingTapCreate(CFAllocator?, UnsafePointer&lt;MTAudioProcessingTapCallbacks>, MTAudioProcessingTapCreationFlags, UnsafeMutablePointer&lt;Unmanaged&lt;MTAudioProcessingTap>?>) -> OSStatus

Creates a new audio processing tap.

func MTAudioProcessingTapGetSourceAudio(MTAudioProcessingTap, CMItemCount, UnsafeMutablePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;MTAudioProcessingTapFlags>?, UnsafeMutablePointer&lt;CMTimeRange>?, UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves source audio for an audio processing tap.

func MTAudioProcessingTapGetStorage(MTAudioProcessingTap) -> UnsafeMutableRawPointer

Retrieves a custom storage pointer for an audio processing tap.

func MTAudioProcessingTapGetTypeID() -> CFTypeID

Retrieves the type identifier for this audio processing tap.

class MTAudioProcessingTap

An audio processing tap object.

