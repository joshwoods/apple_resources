

- IOBluetooth
-  IOBluetoothNSStringFromDeviceAddress(\_:) 

Function

# IOBluetoothNSStringFromDeviceAddress(\_:)

Convenience routine to take a device address structure and create an NSString.

macOS

``` source
func IOBluetoothNSStringFromDeviceAddress(_ deviceAddress: UnsafePointer!) -> String!
```

## Parameters 

`deviceAddress`  

A valid bluetooth device structure.

## Return Value

Returns the created address string.

## Discussion

The resultant string will be in this format: “00-11-22-33-44-55”

## See Also

### Miscellaneous

func IOBluetoothFindNumberOfRegistryEntriesOfClassName(UnsafePointer&lt;CChar>!) -> Int

The number of registry entries with a device classname.

func IOBluetoothGetUniqueFileNameAndPath(String!, String!) -> String!

func IOBluetoothIsFileAppleDesignatedPIMData(String!) -> Bool

Apple designated PIM data is classified as: .vcard, .vcal, .vcf, .vnote, .vmsg, .vcs

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

