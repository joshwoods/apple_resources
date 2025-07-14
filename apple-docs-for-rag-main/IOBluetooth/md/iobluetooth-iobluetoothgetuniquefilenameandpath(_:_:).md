

- IOBluetooth
-  IOBluetoothGetUniqueFileNameAndPath(\_:\_:) 

Function

# IOBluetoothGetUniqueFileNameAndPath(\_:\_:)

macOS

``` source
func IOBluetoothGetUniqueFileNameAndPath(
    _ inName: String!,
    _ inPath: String!
) -> String!
```

## Parameters 

`inName`  

Name of file that needs unique name in the specified path.

`inPath`  

Path you are trying to put file into.

## Return Value

String with a unique name appended on it for the provided path.

## Discussion

When passed a VALID filename and a VALID path, this routine will return you a the path with the name appended onto it. If it already exist, it will insert a \#1, \#2, etc. Example: If you pass @“TestFile.txt” and @”~/Documents”, you will get @“~Documents/TestFile.txt”. If one already exists, you will be returned: @“~Documents/TestFile \#1.txt”.

## See Also

### Miscellaneous

func IOBluetoothFindNumberOfRegistryEntriesOfClassName(UnsafePointer&lt;CChar>!) -> Int

The number of registry entries with a device classname.

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

