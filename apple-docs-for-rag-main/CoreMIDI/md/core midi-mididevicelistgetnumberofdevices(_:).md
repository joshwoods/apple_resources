

- Core MIDI
-  MIDIDeviceListGetNumberOfDevices(\_:) 

Function

# MIDIDeviceListGetNumberOfDevices(\_:)

Retrieves the number of devices in a device list.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIDeviceListGetNumberOfDevices(_ devList: MIDIDeviceListRef) -> Int
```

## Parameters 

`devList`  

The device list.

## Return Value

The number of devices in the list, or 0 if an error occurred.

## See Also

### Managing Device Lists

func MIDIDeviceListGetDevice(MIDIDeviceListRef, Int) -> MIDIDeviceRef

Retrieves a MIDI device from a device list.

func MIDIDeviceListAddDevice(MIDIDeviceListRef, MIDIDeviceRef) -> OSStatus

Adds the specified device to the device list.

func MIDIDeviceListDispose(MIDIDeviceListRef) -> OSStatus

Disposes of a device list, but not its devices.

typealias MIDIDeviceListRef

A list of MIDI devices.

