

- Audio Toolbox
-  AudioUnitSetParameter(\_:\_:\_:\_:\_:\_:) 

Function

# AudioUnitSetParameter(\_:\_:\_:\_:\_:\_:)

Sets the value of an audio unit parameter.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitSetParameter(
    _ inUnit: AudioUnit,
    _ inID: AudioUnitParameterID,
    _ inScope: AudioUnitScope,
    _ inElement: AudioUnitElement,
    _ inValue: AudioUnitParameterValue,
    _ inBufferOffsetInFrames: UInt32
) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit that you want to set a parameter value for.

`inID`  

The audio unit parameter identifier.

`inScope`  

The audio unit scope for the parameter.

`inElement`  

The audio unit element for the parameter.

`inValue`  

The value that you want to apply to the parameter.

`inBufferOffsetInFrames`  

Set this to 0. To schedule the setting of a parameter value, use the AudioUnitScheduleParameters(_:_:_:) function.

## Return Value

A result code.

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## See Also

### Getting and Setting Parameters

func AudioUnitGetParameter(AudioUnit, AudioUnitParameterID, AudioUnitScope, AudioUnitElement, UnsafeMutablePointer&lt;AudioUnitParameterValue>) -> OSStatus

Gets the value of an audio unit parameter.

func AudioUnitScheduleParameters(AudioUnit, UnsafePointer&lt;AudioUnitParameterEvent>, UInt32) -> OSStatus

Schedules changes to the value of an audio unit parameter.

