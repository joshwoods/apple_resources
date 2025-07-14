

- Media Toolbox
-  MTAudioProcessingTapGetTypeID() 

Function

# MTAudioProcessingTapGetTypeID()

Retrieves the type identifier for this audio processing tap.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func MTAudioProcessingTapGetTypeID() -> CFTypeID
```

## See Also

### Audio Taps

func MTAudioProcessingTapCreate(CFAllocator?, UnsafePointer&lt;MTAudioProcessingTapCallbacks>, MTAudioProcessingTapCreationFlags, UnsafeMutablePointer&lt;Unmanaged&lt;MTAudioProcessingTap>?>) -> OSStatus

Creates a new audio processing tap.

func MTAudioProcessingTapGetSourceAudio(MTAudioProcessingTap, CMItemCount, UnsafeMutablePointer&lt;AudioBufferList>, UnsafeMutablePointer&lt;MTAudioProcessingTapFlags>?, UnsafeMutablePointer&lt;CMTimeRange>?, UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves source audio for an audio processing tap.

func MTAudioProcessingTapGetStorage(MTAudioProcessingTap) -> UnsafeMutableRawPointer

Retrieves a custom storage pointer for an audio processing tap.

typealias MTAudioProcessingTapFlags

Flags that indicate where to tap the audio.

class MTAudioProcessingTap

An audio processing tap object.

