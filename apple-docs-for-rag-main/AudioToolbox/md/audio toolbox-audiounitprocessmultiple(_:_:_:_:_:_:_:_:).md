

- Audio Toolbox
-  AudioUnitProcessMultiple(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# AudioUnitProcessMultiple(\_:\_:\_:\_:\_:\_:\_:\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitProcessMultiple(
    _ inUnit: AudioUnit,
    _ ioActionFlags: UnsafeMutablePointer?,
    _ inTimeStamp: UnsafePointer,
    _ inNumberFrames: UInt32,
    _ inNumberInputBufferLists: UInt32,
    _ inInputBufferLists: UnsafeMutablePointer>,
    _ inNumberOutputBufferLists: UInt32,
    _ ioOutputBufferLists: UnsafeMutablePointer>
) -> OSStatus
```

## See Also

### Initializing the Audio Unit

func AudioUnitInitialize(AudioUnit) -> OSStatus

Initializes an audio unit

func AudioUnitUninitialize(AudioUnit) -> OSStatus

Uninitializes an audio unit.

func AudioUnitProcess(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

func AudioUnitReset(AudioUnit, AudioUnitScope, AudioUnitElement) -> OSStatus

Resets an audio unit’s render state.

typealias AudioUnit

The data type for a plug-in component that provides audio processing or audio data generation.

