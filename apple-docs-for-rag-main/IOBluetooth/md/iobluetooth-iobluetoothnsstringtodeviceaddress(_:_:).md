

- IOBluetooth
-  IOBluetoothNSStringToDeviceAddress(\_:\_:) 

Function

# IOBluetoothNSStringToDeviceAddress(\_:\_:)

Convenience routine to take an NSString and turn it into a BluetoothDeviceAddress structure.

macOS

``` source
func IOBluetoothNSStringToDeviceAddress(
    _ inNameString: String!,
    _ outDeviceAddress: UnsafeMutablePointer!
) -> IOReturn
```

## Parameters 

`inNameString`  

Ptr to an NSString that contains the data to turn into the device address.

`outDeviceAddress`  

Ptr to an address structure that will be returned.

## Return Value

Returns success (0) or failure code.

## Discussion

Pass in most types of strings, such as “001122334455” or “00-11-22-33-44-55” and the conversion should be successful. Also, you should have 2 characters per byte for the conversion to work properly.

## See Also

### Miscellaneous

func IOBluetoothFindNumberOfRegistryEntriesOfClassName(UnsafePointer&lt;CChar>!) -> Int

The number of registry entries with a device classname.

func IOBluetoothGetUniqueFileNameAndPath(String!, String!) -> String!

func IOBluetoothIsFileAppleDesignatedPIMData(String!) -> Bool

Apple designated PIM data is classified as: .vcard, .vcal, .vcf, .vnote, .vmsg, .vcs

func IOBluetoothNSStringFromDeviceAddress(UnsafePointer&lt;BluetoothDeviceAddress>!) -> String!

Convenience routine to take a device address structure and create an NSString.

func IOBluetoothNumberOfAvailableHIDDevices() -> Int

Returns total number of HID devices on the system (Bluetooth + USB)

func IOBluetoothNumberOfKeyboardHIDDevices() -> Int

Returns number of keyboard HID devices on the system (Bluetooth + USB)

func IOBluetoothNumberOfPointingHIDDevices() -> Int

Returns number of “pointing” HID devices on the system (Bluetooth + USB)

func IOBluetoothNumberOfTabletHIDDevices() -> Int

Returns number of “Tablet” HID devices on the system (Bluetooth + USB)

