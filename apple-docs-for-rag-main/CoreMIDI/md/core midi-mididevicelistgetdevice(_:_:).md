

- Core MIDI
-  MIDIDeviceListGetDevice(\_:\_:) 

Function

# MIDIDeviceListGetDevice(\_:\_:)

Retrieves a MIDI device from a device list.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0+visionOS 1.0+

``` source
func MIDIDeviceListGetDevice(
    _ devList: MIDIDeviceListRef,
    _ index0: Int
) -> MIDIDeviceRef
```

## Parameters 

`devList`  

The device list.

`index0`  

The index of the device to return.

## Return Value

A reference to a device, or `NULL` if an error occurred.

## See Also

### Managing Device Lists

func MIDIDeviceListGetNumberOfDevices(MIDIDeviceListRef) -> Int

Retrieves the number of devices in a device list.

func MIDIDeviceListAddDevice(MIDIDeviceListRef, MIDIDeviceRef) -> OSStatus

Adds the specified device to the device list.

func MIDIDeviceListDispose(MIDIDeviceListRef) -> OSStatus

Disposes of a device list, but not its devices.

typealias MIDIDeviceListRef

A list of MIDI devices.

