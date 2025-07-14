

- Core MIDI
-  MIDIDeviceListRef 

Type Alias

# MIDIDeviceListRef

A list of MIDI devices.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDIDeviceListRef = MIDIObjectRef
```

## Discussion

This object doesn’t own the devices, so disposing it doesn’t dispose the devices it references.

## See Also

### Managing Device Lists

func MIDIDeviceListGetNumberOfDevices(MIDIDeviceListRef) -> Int

Retrieves the number of devices in a device list.

func MIDIDeviceListGetDevice(MIDIDeviceListRef, Int) -> MIDIDeviceRef

Retrieves a MIDI device from a device list.

func MIDIDeviceListAddDevice(MIDIDeviceListRef, MIDIDeviceRef) -> OSStatus

Adds the specified device to the device list.

func MIDIDeviceListDispose(MIDIDeviceListRef) -> OSStatus

Disposes of a device list, but not its devices.

