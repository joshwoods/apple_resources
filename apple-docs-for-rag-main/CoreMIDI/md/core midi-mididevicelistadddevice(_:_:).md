

- Core MIDI
-  MIDIDeviceListAddDevice(\_:\_:) 

Function

# MIDIDeviceListAddDevice(\_:\_:)

Adds the specified device to the device list.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIDeviceListAddDevice(
    _ devList: MIDIDeviceListRef,
    _ dev: MIDIDeviceRef
) -> OSStatus
```

## Parameters 

`devList`  

The device list.

`dev`  

The device to add to the list.

## Return Value

An `OSStatus` result code.

## See Also

### Managing Device Lists

func MIDIDeviceListGetNumberOfDevices(MIDIDeviceListRef) -> Int

Retrieves the number of devices in a device list.

func MIDIDeviceListGetDevice(MIDIDeviceListRef, Int) -> MIDIDeviceRef

Retrieves a MIDI device from a device list.

func MIDIDeviceListDispose(MIDIDeviceListRef) -> OSStatus

Disposes of a device list, but not its devices.

typealias MIDIDeviceListRef

A list of MIDI devices.

