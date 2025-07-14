

- IOBluetooth
- IOBluetoothDevice
-  addToFavorites() 

Instance Method

# addToFavorites()

Adds the target device to the user’s favorite devices list.

macOS

``` source
func addToFavorites() -> IOReturn
```

## Return Value

Returns kIOReturnSuccess if the device was successfully added to the user’s list of favorite devices.

## Discussion

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

