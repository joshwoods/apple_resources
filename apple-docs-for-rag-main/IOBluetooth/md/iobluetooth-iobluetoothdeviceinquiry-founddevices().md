

- IOBluetooth
- IOBluetoothDeviceInquiry
-  foundDevices() 

Instance Method

# foundDevices()

Returns found IOBluetoothDevice objects as an array.

macOS

``` source
func foundDevices() -> [Any]!
```

## Return Value

Returns an NSArray of IOBluetoothDevice objects.

## Discussion

Will not return nil. If there are no devices found, returns an array with length of 0.

