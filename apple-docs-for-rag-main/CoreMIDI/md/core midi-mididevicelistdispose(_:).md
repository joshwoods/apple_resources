

- Core MIDI
-  MIDIDeviceListDispose(\_:) 

Function

# MIDIDeviceListDispose(\_:)

Disposes of a device list, but not its devices.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDIDeviceListDispose(_ devList: MIDIDeviceListRef) -> OSStatus
```

## Parameters 

`devList`  

The device list of which you dispose.

## Return Value

An `OSStatus` result code.

## See Also

### Managing Device Lists

func MIDIDeviceListGetNumberOfDevices(MIDIDeviceListRef) -> Int

Retrieves the number of devices in a device list.

func MIDIDeviceListGetDevice(MIDIDeviceListRef, Int) -> MIDIDeviceRef

Retrieves a MIDI device from a device list.

func MIDIDeviceListAddDevice(MIDIDeviceListRef, MIDIDeviceRef) -> OSStatus

Adds the specified device to the device list.

typealias MIDIDeviceListRef

A list of MIDI devices.

