

- IOBluetooth
- IOBluetoothDevice
-  getPageScanPeriodMode() 

Instance Method

# getPageScanPeriodMode()

Get the value of the page scan period mode for the device.

macOS

``` source
func getPageScanPeriodMode() -> BluetoothPageScanPeriodMode
```

## Return Value

Returns page scan period mode value for the device.

## Discussion

This value is only meaningful if the target device has been seen during an inquiry. This can be by checking the result of -getLastInquiryUpdate. If nil is returned, then the device hasn’t been seen.

