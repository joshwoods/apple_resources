

- Audio Toolbox
-  AudioUnitSetProperty(\_:\_:\_:\_:\_:\_:) 

Function

# AudioUnitSetProperty(\_:\_:\_:\_:\_:\_:)

Sets the value of an audio unit property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitSetProperty(
    _ inUnit: AudioUnit,
    _ inID: AudioUnitPropertyID,
    _ inScope: AudioUnitScope,
    _ inElement: AudioUnitElement,
    _ inData: UnsafeRawPointer?,
    _ inDataSize: UInt32
) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit that you want to set a property value for.

`inID`  

The audio unit property identifier.

`inScope`  

The audio unit scope for the property.

`inElement`  

The audio unit element for the property.

`inData`  

The value that you want to apply to the property. May be `NULL` (see Discussion).

Always pass property values by reference. For example, for a property value of type `CFStringRef`, pass it as `&myCFString`.

`inDataSize`  

The size of the data you are providing in the `inData` parameter.

## Return Value

A result code.

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## Discussion

To clear an audio unit property value, set the `inData` parameter to `NULL` and set the `inDataSize` parameter to `0`. Clearing properties works only for those properties that do not have a default value.

## See Also

### Configuring Audio Unit Properties

func AudioUnitGetProperty(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the value of an audio unit property.

func AudioUnitGetPropertyInfo(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an audio unit property.

func AudioUnitAddPropertyListener(AudioUnit, AudioUnitPropertyID, AudioUnitPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback to receive audio unit property change notifications.

func AudioUnitRemovePropertyListenerWithUserData(AudioUnit, AudioUnitPropertyID, AudioUnitPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Unregisters a previously-registered property listener callback function.

