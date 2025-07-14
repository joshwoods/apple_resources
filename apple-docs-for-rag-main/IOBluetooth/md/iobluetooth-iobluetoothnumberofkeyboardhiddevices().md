

- IOBluetooth
-  IOBluetoothNumberOfKeyboardHIDDevices() 

Function

# IOBluetoothNumberOfKeyboardHIDDevices()

Returns number of keyboard HID devices on the system (Bluetooth + USB)

macOS

``` source
func IOBluetoothNumberOfKeyboardHIDDevices() -> Int
```

## Return Value

Number of HID devices.

## See Also

### Miscellaneous

func IOBluetoothFindNumberOfRegistryEntriesOfClassName(UnsafePointer&lt;CChar>!) -> Int

The number of registry entries with a device classname.

func IOBluetoothGetUniqueFileNameAndPath(String!, String!) -> String!

func IOBluetoothIsFileAppleDesignatedPIMData(String!) -> Bool

Apple designated PIM data is classified as: .vcard, .vcal, .vcf, .vnote, .vmsg, .vcs

func IOBluetoothNSStringFromDeviceAddress(UnsafePointer&lt;BluetoothDeviceAddress>!) -> String!

Convenience routine to take a device address structure and create an NSString.

func IOBluetoothNSStringToDeviceAddress(String!, UnsafeMutablePointer&lt;BluetoothDeviceAddress>!) -> IOReturn

Convenience routine to take an NSString and turn it into a BluetoothDeviceAddress structure.

func IOBluetoothNumberOfAvailableHIDDevices() -> Int

Returns total number of HID devices on the system (Bluetooth + USB)

func IOBluetoothNumberOfPointingHIDDevices() -> Int

Returns number of “pointing” HID devices on the system (Bluetooth + USB)

func IOBluetoothNumberOfTabletHIDDevices() -> Int

Returns number of “Tablet” HID devices on the system (Bluetooth + USB)

