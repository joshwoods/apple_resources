

- Audio Toolbox
-  AudioUnitInitialize(\_:) 

Function

# AudioUnitInitialize(\_:)

Initializes an audio unit

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitInitialize(_ inUnit: AudioUnit) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit to initialize.

## Return Value

A result code.

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## Discussion

On successful initialization, the audio formats for input and output are valid and the audio unit is ready to render. During initialization, an audio unit allocates memory according to the maximum number of audio frames it can produce in response to a single render call.

Usually, the state of an audio unit (such as its I/O formats and memory allocations) cannot be changed while an audio unit is initialized.

## See Also

### Initializing the Audio Unit

func AudioUnitUninitialize(AudioUnit) -> OSStatus

Uninitializes an audio unit.

func AudioUnitProcess(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

func AudioUnitProcessMultiple(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;UnsafePointer&lt;AudioBufferList>>, UInt32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AudioBufferList>>) -> OSStatus

func AudioUnitReset(AudioUnit, AudioUnitScope, AudioUnitElement) -> OSStatus

Resets an audio unit’s render state.

typealias AudioUnit

The data type for a plug-in component that provides audio processing or audio data generation.

