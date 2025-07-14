

- IOBluetooth
- IOBluetoothDevice
-  removeFromFavorites() 

Instance Method

# removeFromFavorites()

Removes the target device from the user’s favorite devices list.

macOS

``` source
func removeFromFavorites() -> IOReturn
```

## Return Value

Returns kIOReturnSuccess if the device was successfully removed from the user’s list of favorite devices.

## Discussion

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

