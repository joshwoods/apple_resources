

- IOBluetooth
- IOBluetoothHostController
-  setClassOfDevice(\_:forTimeInterval:) 

Instance Method

# setClassOfDevice(\_:forTimeInterval:)

Sets the current class of device value, for the specified amount of time. Note that the time interval *must* be set and valid. The range of acceptable values is 30-120 seconds. Anything above or below will be rounded up, or down, as appropriate.

macOS

``` source
func setClassOfDevice(
    _ classOfDevice: BluetoothClassOfDevice,
    forTimeInterval seconds: TimeInterval
) -> IOReturn
```

## Return Value

Returns the whether setting the class of device value was successful. 0 if success, error code otherwise.

