

- Audio Toolbox
-  AudioUnitGetProperty(\_:\_:\_:\_:\_:\_:) 

Function

# AudioUnitGetProperty(\_:\_:\_:\_:\_:\_:)

Gets the value of an audio unit property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitGetProperty(
    _ inUnit: AudioUnit,
    _ inID: AudioUnitPropertyID,
    _ inScope: AudioUnitScope,
    _ inElement: AudioUnitElement,
    _ outData: UnsafeMutableRawPointer,
    _ ioDataSize: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit that you want to get a property value from.

`inID`  

The identifier for the property.

`inScope`  

The audio unit scope for the property.

`inElement`  

The audio unit element for the property.

`outData`  

On successful output, the current value for the specified audio unit property. Set this parameter to `NULL` when calling this function if you only want to determine how much memory to allocate for a variable size property.

`ioDataSize`  

On input, the expected size of the property value, as pointed to by the `outData` parameter. On output, the size of the data that was returned.

## Return Value

A result code.

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## Discussion

Some Core Audio property values are C types and others are Core Foundation objects.

If you call this function to retrieve a value that is a Core Foundation object, then this function—despite the use of “Get” in its name—duplicates the object. You are responsible for releasing the object, as described in The Create Rule in Memory Management Programming Guide for Core Foundation.

## See Also

### Configuring Audio Unit Properties

func AudioUnitSetProperty(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeRawPointer?, UInt32) -> OSStatus

Sets the value of an audio unit property.

func AudioUnitGetPropertyInfo(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an audio unit property.

func AudioUnitAddPropertyListener(AudioUnit, AudioUnitPropertyID, AudioUnitPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback to receive audio unit property change notifications.

func AudioUnitRemovePropertyListenerWithUserData(AudioUnit, AudioUnitPropertyID, AudioUnitPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Unregisters a previously-registered property listener callback function.

