

- Core MIDI
-  MIDIDeviceDispose(\_:) 

Function

# MIDIDeviceDispose(\_:)

Disposes of a MIDI device.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.3+visionOS 1.0+

``` source
func MIDIDeviceDispose(_ device: MIDIDeviceRef) -> OSStatus
```

## Parameters 

`device`  

The device to dispose.

## Return Value

An `OSStatus` result code.

## Discussion

Drivers may call this function to dispose of device objects that they haven’t already added to the system using MIDISetupAddDevice(_:). To remove a device after adding it to the session, call MIDISetupRemoveDevice(_:).

Nondrivers can’t call this function, and instead must call MIDISetupAddDevice(_:) and MIDISetupRemoveDevice(_:).

## See Also

### Managing Device Lifecyle

func MIDIDeviceCreate(MIDIDriverRef?, CFString, CFString, CFString, UnsafeMutablePointer&lt;MIDIDeviceRef>) -> OSStatus

Creates a new device object that corresponds to the available hardware.

typealias MIDIDeviceRef

A MIDI device that contains entities.

