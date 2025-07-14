

- Core MIDI
- MIDICIDeviceIdentification
-  reserved 

Instance Property

# reserved

A reserved field whose value is always zero.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8)
```

## See Also

### Configuring Device Identification

var manufacturer: (UInt8, UInt8, UInt8)

The MIDI System Exclusive (SysEx) ID of the device manufacturer.

var modelNumber: (UInt8, UInt8)

The device model number.

var family: (UInt8, UInt8)

The group of familes to which the device belongs.

var revisionLevel: (UInt8, UInt8, UInt8, UInt8)

The revision number of the device model number.

