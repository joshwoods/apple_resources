

- Core MIDI
-  MIDISetupAddExternalDevice(\_:) 

Function

# MIDISetupAddExternalDevice(\_:)

Adds an external MIDI device to the current MIDI setup.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDISetupAddExternalDevice(_ device: MIDIDeviceRef) -> OSStatus
```

## Parameters 

`device`  

The device to add.

## Return Value

An `OSStatus` result code.

## See Also

### Managing External Devices

func MIDIExternalDeviceCreate(CFString, CFString, CFString, UnsafeMutablePointer&lt;MIDIDeviceRef>) -> OSStatus

Creates an external MIDI device.

func MIDISetupRemoveExternalDevice(MIDIDeviceRef) -> OSStatus

Removes an external MIDI device from the current MIDI setup.

