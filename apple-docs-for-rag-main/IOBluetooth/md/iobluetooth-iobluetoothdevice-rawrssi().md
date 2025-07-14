

- IOBluetooth
- IOBluetoothDevice
-  rawRSSI() 

Instance Method

# rawRSSI()

Get the raw RSSI device (if connected).

macOS 10.7+

``` source
func rawRSSI() -> BluetoothHCIRSSIValue
```

## Return Value

Returns the raw RSSI of the device.

## Discussion

This value is the perceived RSSI value, not relative the the golden range (see getRSSI for that value). This value will not available on all Bluetooth modules. If the value cannot be read (e.g. the device is disconnected) or is not available on a module, a value of +127 will be returned.

