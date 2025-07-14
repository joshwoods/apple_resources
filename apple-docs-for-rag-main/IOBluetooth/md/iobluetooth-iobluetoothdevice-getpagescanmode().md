

- IOBluetooth
- IOBluetoothDevice
-  getPageScanMode() 

Instance Method

# getPageScanMode()

Get the page scan mode for the device.

macOS

``` source
func getPageScanMode() -> BluetoothPageScanMode
```

## Return Value

Returns the value for the page scan mode for the device.

## Discussion

This value is only meaningful if the target device has been seen during an inquiry. This can be by checking the result of -getLastInquiryUpdate. If nil is returned, then the device hasn’t been seen.

