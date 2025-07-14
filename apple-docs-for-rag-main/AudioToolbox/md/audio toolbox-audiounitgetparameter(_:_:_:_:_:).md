

- Audio Toolbox
-  AudioUnitGetParameter(\_:\_:\_:\_:\_:) 

Function

# AudioUnitGetParameter(\_:\_:\_:\_:\_:)

Gets the value of an audio unit parameter.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitGetParameter(
    _ inUnit: AudioUnit,
    _ inID: AudioUnitParameterID,
    _ inScope: AudioUnitScope,
    _ inElement: AudioUnitElement,
    _ outValue: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit that you want to get a parameter value from.

`inID`  

The identifier for the parameter.

`inScope`  

The audio unit scope for the parameter.

`inElement`  

The audio unit element for the parameter.

`outValue`  

On success, contains the current value for the specified audio unit parameter.

## Return Value

A result code.

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## See Also

### Getting and Setting Parameters

func AudioUnitScheduleParameters(AudioUnit, UnsafePointer&lt;AudioUnitParameterEvent>, UInt32) -> OSStatus

Schedules changes to the value of an audio unit parameter.

func AudioUnitSetParameter(AudioUnit, AudioUnitParameterID, AudioUnitScope, AudioUnitElement, AudioUnitParameterValue, UInt32) -> OSStatus

Sets the value of an audio unit parameter.

