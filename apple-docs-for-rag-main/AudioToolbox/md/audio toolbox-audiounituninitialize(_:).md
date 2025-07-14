

- Audio Toolbox
-  AudioUnitUninitialize(\_:) 

Function

# AudioUnitUninitialize(\_:)

Uninitializes an audio unit.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitUninitialize(_ inUnit: AudioUnit) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit that you want to uninitialize.

## Return Value

A result code.

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## Discussion

Before you change an initialize audio unit’s processing characteristics, such as its input or output audio data format or its sample rate, you must first uninitialize it. Calling this function deallocates the audio unit’s resources.

After calling this function, you can reconfigure the audio unit and then call AudioUnitInitialize(_:) to reinitialize it.

## See Also

### Initializing the Audio Unit

func AudioUnitInitialize(AudioUnit) -> OSStatus

Initializes an audio unit

func AudioUnitProcess(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

func AudioUnitProcessMultiple(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;UnsafePointer&lt;AudioBufferList>>, UInt32, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AudioBufferList>>) -> OSStatus

func AudioUnitReset(AudioUnit, AudioUnitScope, AudioUnitElement) -> OSStatus

Resets an audio unit’s render state.

typealias AudioUnit

The data type for a plug-in component that provides audio processing or audio data generation.

