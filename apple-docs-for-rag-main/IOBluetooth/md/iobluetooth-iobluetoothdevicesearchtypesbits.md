

- IOBluetooth
-  IOBluetoothDeviceSearchTypesBits 

Structure

# IOBluetoothDeviceSearchTypesBits

Bits to determine what Bluetooth devices to search for

macOS

``` source
struct IOBluetoothDeviceSearchTypesBits
```

## Overview

You can search for general device classes and service classes, or you can search for a specific device address or name. If you pass NULL as the attribute structure, you will get ALL devices in the vicinity found during a search. Note that passing a zeroed out block of attributes is NOT equivalent to passing in NULL!

## Topics

### Constants

var kIOBluetoothDeviceSearchClassic: IOBluetoothDeviceSearchTypesBits

var kIOBluetoothDeviceSearchLE: IOBluetoothDeviceSearchTypesBits

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data Types

typealias BluetoothAFHMode

typealias BluetoothAirMode

typealias BluetoothAllowRoleSwitch

typealias BluetoothAuthenticationRequirements

struct BluetoothAuthenticationRequirementsValues

typealias BluetoothClassOfDevice

typealias BluetoothClockOffset

struct BluetoothCompanyIdentifers

typealias BluetoothConnectionHandle

typealias BluetoothDeviceClassMajor

typealias BluetoothDeviceClassMinor

typealias BluetoothDeviceName

typealias BluetoothEncryptionEnable

struct BluetoothFeatureBits

typealias BluetoothHCIACLDataByteCount

