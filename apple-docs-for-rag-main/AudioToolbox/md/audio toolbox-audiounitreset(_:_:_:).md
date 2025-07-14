

- Audio Toolbox
-  AudioUnitReset(\_:\_:\_:) 

Function

# AudioUnitReset(\_:\_:\_:)

Resets an audio unit’s render state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitReset(
    _ inUnit: AudioUnit,
    _ inScope: AudioUnitScope,
    _ inElement: AudioUnitElement
) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit whose render state you are resetting.

`inScope`  

The audio unit scope, typically set to `kAudioUnitScope_Global`.

`inElement`  

The audio unit element, typically set to `0`.

## Return Value

A result code.

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## Discussion

This function resets the render state of an audio unit. For example, with a delay or reverb type of audio unit, it clears all of the delay lines maintained within the audio unit. Typically, you call this function when an audio unit was previously rendering and was taken out of the render chain (for example, if the track it is in gets muted) and is now being added back in (for example, unmuted). Your application should reset the audio unit before adding it back to the render chain so that it does not produce audio from its delay lines that is no longer valid.

This function clears memory. It does not allocate or free memory resources.

## See Also

### Initializing the Audio Unit

func AudioUnitInitialize(AudioUnit) -> OSStatus

Initializes an audio unit

func AudioUnitUninitialize(AudioUnit) -> OSStatus

Uninitializes an audio unit.

func AudioUnitProcess(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

func AudioUnitProcessMultiple(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;UnsafePointer&lt;AudioBufferList>>, UInt32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AudioBufferList>>) -> OSStatus

typealias AudioUnit

The data type for a plug-in component that provides audio processing or audio data generation.

