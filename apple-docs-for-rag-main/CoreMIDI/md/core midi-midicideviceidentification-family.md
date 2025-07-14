

- Core MIDI
- MIDICIDeviceIdentification
-  family 

Instance Property

# family

The group of familes to which the device belongs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var family: (UInt8, UInt8)
```

## Discussion

This value is 2 bytes long.

## See Also

### Configuring Device Identification

var manufacturer: (UInt8, UInt8, UInt8)

The MIDI System Exclusive (SysEx) ID of the device manufacturer.

var modelNumber: (UInt8, UInt8)

The device model number.

var revisionLevel: (UInt8, UInt8, UInt8, UInt8)

The revision number of the device model number.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8)

A reserved field whose value is always zero.

