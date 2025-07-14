

- Core MIDI
- MIDICIDeviceIdentification
-  manufacturer 

Instance Property

# manufacturer

The MIDI System Exclusive (SysEx) ID of the device manufacturer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var manufacturer: (UInt8, UInt8, UInt8)
```

## Discussion

This value is 3 bytes long.

The framework pads single-byte System Exclusive (SysEx) IDs with trailing zeros. For example, Apple’s SysEx ID, 0x11, is `0x110000`.

## See Also

### Configuring Device Identification

var modelNumber: (UInt8, UInt8)

The device model number.

var family: (UInt8, UInt8)

The group of familes to which the device belongs.

var revisionLevel: (UInt8, UInt8, UInt8, UInt8)

The revision number of the device model number.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8)

A reserved field whose value is always zero.

