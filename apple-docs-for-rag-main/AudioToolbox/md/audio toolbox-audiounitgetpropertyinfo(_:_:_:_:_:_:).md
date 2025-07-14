

- Audio Toolbox
-  AudioUnitGetPropertyInfo(\_:\_:\_:\_:\_:\_:) 

Function

# AudioUnitGetPropertyInfo(\_:\_:\_:\_:\_:\_:)

Gets information about an audio unit property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitGetPropertyInfo(
    _ inUnit: AudioUnit,
    _ inID: AudioUnitPropertyID,
    _ inScope: AudioUnitScope,
    _ inElement: AudioUnitElement,
    _ outDataSize: UnsafeMutablePointer?,
    _ outWritable: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit that you want to get property information from.

`inID`  

The identifier for the property.

`inScope`  

The audio unit scope for the property.

`inElement`  

The audio unit element for the property.

`outDataSize`  

On successful output, the maximum size for the audio unit property. Can be `NULL` on input, in which case no value is returned.

`outWritable`  

On successful output, a Boolean value indicating whether the property can be written to (true) or not (false). Can be `NULL` on input, in which case no value is returned.

## Return Value

A result code.

## Discussion

Some properties that have read/write access when an audio unit is uninitialized become read-only when the audio unit is initialized.

## See Also

### Configuring Audio Unit Properties

func AudioUnitGetProperty(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the value of an audio unit property.

func AudioUnitSetProperty(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeRawPointer?, UInt32) -> OSStatus

Sets the value of an audio unit property.

func AudioUnitAddPropertyListener(AudioUnit, AudioUnitPropertyID, AudioUnitPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback to receive audio unit property change notifications.

func AudioUnitRemovePropertyListenerWithUserData(AudioUnit, AudioUnitPropertyID, AudioUnitPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Unregisters a previously-registered property listener callback function.

