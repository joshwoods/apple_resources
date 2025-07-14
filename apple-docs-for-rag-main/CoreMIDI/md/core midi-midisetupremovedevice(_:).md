

- Core MIDI
-  MIDISetupRemoveDevice(\_:) 

Function

# MIDISetupRemoveDevice(\_:)

Removes a driver-owned MIDI device from the current MIDI setup.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDISetupRemoveDevice(_ device: MIDIDeviceRef) -> OSStatus
```

## Parameters 

`device`  

The device to remove.

## Return Value

An `OSStatus` result code.

## Discussion

Typically, only a studio-configuration editor calls this function to remove a device that’s offline and which the user has specified as permanently missing. It’s a good practice to have drivers set the deviceʼs kMIDIPropertyOffline to 1, instead of removing the device from the setup, so if the device reappears later, the system preserves the deviceʼs property state.

## See Also

### Managing Devices

func MIDISetupAddDevice(MIDIDeviceRef) -> OSStatus

Adds a driver-owned MIDI device to the current MIDI setup.

