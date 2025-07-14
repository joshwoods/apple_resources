

- Audio Toolbox
-  AudioUnitProcess(\_:\_:\_:\_:\_:) 

Function

# AudioUnitProcess(\_:\_:\_:\_:\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitProcess(
    _ inUnit: AudioUnit,
    _ ioActionFlags: UnsafeMutablePointer?,
    _ inTimeStamp: UnsafePointer,
    _ inNumberFrames: UInt32,
    _ ioData: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Initializing the Audio Unit

func AudioUnitInitialize(AudioUnit) -> OSStatus

Initializes an audio unit

func AudioUnitUninitialize(AudioUnit) -> OSStatus

Uninitializes an audio unit.

func AudioUnitProcessMultiple(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;UnsafePointer&lt;AudioBufferList>>, UInt32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AudioBufferList>>) -> OSStatus

func AudioUnitReset(AudioUnit, AudioUnitScope, AudioUnitElement) -> OSStatus

Resets an audio unit’s render state.

typealias AudioUnit

The data type for a plug-in component that provides audio processing or audio data generation.

