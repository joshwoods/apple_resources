

- IOBluetooth
- IOBluetoothDevice
-  getClockOffset() 

Instance Method

# getClockOffset()

Get the clock offset value of the device.

macOS

``` source
func getClockOffset() -> BluetoothClockOffset
```

## Return Value

Returns the clock offset value for the device.

## Discussion

This value is only meaningful if the target device has been seen during an inquiry. This can be by checking the result of -getLastInquiryUpdate. If nil is returned, then the device hasn’t been seen.

