

- Core MIDI
-  MIDISetupAddDevice(\_:) 

Function

# MIDISetupAddDevice(\_:)

Adds a driver-owned MIDI device to the current MIDI setup.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDISetupAddDevice(_ device: MIDIDeviceRef) -> OSStatus
```

## Parameters 

`device`  

The device to add.

## Return Value

An `OSStatus` result code.

## Discussion

Only MIDI drivers may call this function.

## See Also

### Managing Devices

func MIDISetupRemoveDevice(MIDIDeviceRef) -> OSStatus

Removes a driver-owned MIDI device from the current MIDI setup.

