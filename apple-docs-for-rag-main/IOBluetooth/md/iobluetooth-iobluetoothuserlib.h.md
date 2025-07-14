

- IOBluetooth
-  IOBluetoothUserLib.h 

API Collection

# IOBluetoothUserLib.h

Public Interfaces for Apple’s implementation of Bluetooth technology.

## Overview

There is an accompanying header to this, “Bluetooth.h”, which contains all technology-specific typedefs and information. This header relies heavily on it.

### Included Headers

- \

- \

- \

- \

## Topics

### Miscellaneous

func IOBluetoothIgnoreHIDDevice(IOBluetoothDeviceRef!)

Hints that the macOS Bluetooth software should ignore a HID device that connects up.

func IOBluetoothL2CAPChannelRegisterForChannelCloseNotification(IOBluetoothL2CAPChannelRef!, IOBluetoothUserNotificationCallback!, UnsafeMutableRawPointer!) -> Unmanaged&lt;IOBluetoothUserNotificationRef>!

Allows a client to register for a channel close notification.

func IOBluetoothRemoveIgnoredHIDDevice(IOBluetoothDeviceRef!)

The counterpart to the above IOBluetoothIgnoreHIDDevice() API.

func IOBluetoothUserNotificationUnregister(IOBluetoothUserNotificationRef!)

Unregisters the target notification.

### Callbacks

See the Overview for header-level documentation.

typealias IOBluetoothUserNotificationCallback

Callback function definition for user notifications.

### Data Types

See the Overview for header-level documentation.

typealias IOBluetoothDeviceSearchOptions

struct IOBluetoothDeviceSearchAttributes

Structure used to search for particular devices.

struct IOBluetoothDeviceSearchDeviceAttributes

Structure used to search for particular devices.

### Constants

See the Overview for header-level documentation.

struct IOBluetoothDeviceSearchDeviceAttributes

Structure used to search for particular devices.

struct IOBluetoothDeviceSearchTypesBits

Bits to determine what Bluetooth devices to search for

## See Also

### Reference

Bluetooth.h User-Space

Bluetooth wireless technology

IOBluetoothUtilities.h

See the Overview section above for header-level documentation.

OBEX.h

Public OBEX technology interfaces.

OBEXBluetooth.h

Object Exchange over Bluetooth.

OBEXFileTransferServices.h

IOBluetooth Structures

IOBluetooth Enumerations

IOBluetooth Constants

IOBluetooth Functions

IOBluetooth Data Types

