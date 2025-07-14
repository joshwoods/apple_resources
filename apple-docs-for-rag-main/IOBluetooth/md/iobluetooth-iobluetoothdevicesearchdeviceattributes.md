

- IOBluetooth
-  IOBluetoothDeviceSearchDeviceAttributes 

Structure

# IOBluetoothDeviceSearchDeviceAttributes

Structure used to search for particular devices.

macOS

``` source
struct IOBluetoothDeviceSearchDeviceAttributes
```

## Overview

You can search for general device classes and service classes, or you can search for a specific device address or name. If you pass NULL as the attribute structure, you will get ALL devices in the vicinity found during a search. Note that passing a zeroed out block of attributes is NOT equivalent to passing in NULL!

## Topics

### Initializers

init()

init(address: BluetoothDeviceAddress, name: BluetoothDeviceName, serviceClassMajor: BluetoothServiceClassMajor, deviceClassMajor: BluetoothDeviceClassMajor, deviceClassMinor: BluetoothDeviceClassMinor)

### Instance Properties

var address: BluetoothDeviceAddress

var deviceClassMajor: BluetoothDeviceClassMajor

var deviceClassMinor: BluetoothDeviceClassMinor

var name: BluetoothDeviceName

var serviceClassMajor: BluetoothServiceClassMajor

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Related Documentation

struct IOBluetoothDeviceSearchAttributes

Structure used to search for particular devices.

typealias IOBluetoothDeviceSearchTypes

struct IOBluetoothDeviceSearchTypesBits

Bits to determine what Bluetooth devices to search for

struct IOBluetoothDeviceSearchDeviceAttributes

Structure used to search for particular devices.

### Data Types

typealias IOBluetoothDeviceSearchOptions

struct IOBluetoothDeviceSearchAttributes

Structure used to search for particular devices.

