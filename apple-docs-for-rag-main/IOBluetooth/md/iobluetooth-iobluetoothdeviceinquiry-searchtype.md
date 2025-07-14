

- IOBluetooth
- IOBluetoothDeviceInquiry
-  searchType 

Instance Property

# searchType

Set the devices that are found.

macOS

``` source
var searchType: IOBluetoothDeviceSearchTypes { get set }
```

## Parameters 

`searchType`  

Bluetooth versions the search will discover.

## Discussion

A default of kIOBluetoothDeviceSearchClassic is used, unless a different value is specified using this method.

