

- Audio Toolbox
-  AudioUnitRemovePropertyListenerWithUserData(\_:\_:\_:\_:) 

Function

# AudioUnitRemovePropertyListenerWithUserData(\_:\_:\_:\_:)

Unregisters a previously-registered property listener callback function.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitRemovePropertyListenerWithUserData(
    _ inUnit: AudioUnit,
    _ inID: AudioUnitPropertyID,
    _ inProc: AudioUnitPropertyListenerProc,
    _ inProcUserData: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit that you no longer want to receive property change notifications from.

`inID`  

The identifier for the property that you no longer want to monitor.

`inProc`  

The callback function that you previously registered and are now unregistering.

`inProcUserData`  

The custom data that you provided when registering the callback function.

## Return Value

A result code.

## See Also

### Configuring Audio Unit Properties

func AudioUnitGetProperty(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the value of an audio unit property.

func AudioUnitSetProperty(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeRawPointer?, UInt32) -> OSStatus

Sets the value of an audio unit property.

func AudioUnitGetPropertyInfo(AudioUnit, AudioUnitPropertyID, AudioUnitScope, AudioUnitElement, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;DarwinBoolean>?) -> OSStatus

Gets information about an audio unit property.

func AudioUnitAddPropertyListener(AudioUnit, AudioUnitPropertyID, AudioUnitPropertyListenerProc, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback to receive audio unit property change notifications.

