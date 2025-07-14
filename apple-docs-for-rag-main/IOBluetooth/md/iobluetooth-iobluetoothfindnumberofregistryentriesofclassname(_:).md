

- IOBluetooth
-  IOBluetoothFindNumberOfRegistryEntriesOfClassName(\_:) 

Function

# IOBluetoothFindNumberOfRegistryEntriesOfClassName(\_:)

The number of registry entries with a device classname.

macOS

``` source
func IOBluetoothFindNumberOfRegistryEntriesOfClassName(_ deviceType: UnsafePointer!) -> Int
```

## Return Value

Number of HID devices.

## Overview

Returns total number of registry entries with the provided device classname. For example, IOHIPointing.

## See Also

### Miscellaneous

func IOBluetoothGetUniqueFileNameAndPath(String!, String!) -> String!

func IOBluetoothIsFileAppleDesignatedPIMData(String!) -> Bool

Apple designated PIM data is classified as: .vcard, .vcal, .vcf, .vnote, .vmsg, .vcs

func IOBluetoothNSStringFromDeviceAddress(UnsafePointer&lt;BluetoothDeviceAddress>!) -> String!

Convenience routine to take a device address structure and create an NSString.

func IOBluetoothNSStringToDeviceAddress(String!, UnsafeMutablePointer&lt;BluetoothDeviceAddress>!) -> IOReturn

Convenience routine to take an NSString and turn it into a BluetoothDeviceAddress structure.

func IOBluetoothNumberOfAvailableHIDDevices() -> Int

Returns total number of HID devices on the system (Bluetooth + USB)

func IOBluetoothNumberOfKeyboardHIDDevices() -> Int

Returns number of keyboard HID devices on the system (Bluetooth + USB)

func IOBluetoothNumberOfPointingHIDDevices() -> Int

Returns number of “pointing” HID devices on the system (Bluetooth + USB)

func IOBluetoothNumberOfTabletHIDDevices() -> Int

Returns number of “Tablet” HID devices on the system (Bluetooth + USB)

