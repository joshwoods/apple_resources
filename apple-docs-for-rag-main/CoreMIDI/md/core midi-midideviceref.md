

- Core MIDI
-  MIDIDeviceRef 

Type Alias

# MIDIDeviceRef

A MIDI device that contains entities.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDIDeviceRef = MIDIObjectRef
```

## Discussion

A device object derives from MIDIObjectRef. It doesn’t have an owning object.

## See Also

### Managing Device Lifecyle

func MIDIDeviceCreate(MIDIDriverRef?, CFString, CFString, CFString, UnsafeMutablePointer&lt;MIDIDeviceRef>) -> OSStatus

Creates a new device object that corresponds to the available hardware.

func MIDIDeviceDispose(MIDIDeviceRef) -> OSStatus

Disposes of a MIDI device.

