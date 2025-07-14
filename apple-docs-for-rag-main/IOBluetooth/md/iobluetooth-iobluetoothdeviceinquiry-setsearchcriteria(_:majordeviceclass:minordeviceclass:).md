

- IOBluetooth
- IOBluetoothDeviceInquiry
-  setSearchCriteria(\_:majorDeviceClass:minorDeviceClass:) 

Instance Method

# setSearchCriteria(\_:majorDeviceClass:minorDeviceClass:)

Use this method to set the criteria for the device search.

macOS

``` source
func setSearchCriteria(
    _ inServiceClassMajor: BluetoothServiceClassMajor,
    majorDeviceClass inMajorDeviceClass: BluetoothDeviceClassMajor,
    minorDeviceClass inMinorDeviceClass: BluetoothDeviceClassMinor
)
```

## Parameters 

`inServiceClassMajor`  

Set the major service class for found devices. Set to kBluetoothServiceClassMajorAny for all devices. See BluetoothAssignedNumbers.h for possible values.

`inMajorDeviceClass`  

Set the major device class for found devices. Set to kBluetoothDeviceClassMajorAny for all devices. See BluetoothAssignedNumbers.h for possible values.

`inMinorDeviceClass`  

Set the minor device class for found devices. Set to kBluetoothDeviceClassMinorAny for all devices. See BluetoothAssignedNumbers.h for possible values.

## Discussion

The default inquiry object will search for all types of devices. If you wish to find only keyboards, for example, you might use this method like this:

\[myInquiryObject setSearchCriteria:kBluetoothServiceClassMajorAny majorDeviceClass:kBluetoothDeviceClassMajorPeripheral minorDeviceClass:kBluetoothDeviceClassMinorPeripheral1Keyboard\];

However, we recommend only using this if you are certain of the device class you are looking for, as some devices may report a different/unexpected device class, and the search may miss the device you are interested in.

