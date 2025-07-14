

- IOBluetooth
- IOBluetoothDevice
-  getPageScanRepetitionMode() 

Instance Method

# getPageScanRepetitionMode()

Get the value of the page scan repetition mode for the device.

macOS

``` source
func getPageScanRepetitionMode() -> BluetoothPageScanRepetitionMode
```

## Return Value

Returns the page scan repetition mode value for this device.

## Discussion

This value is only meaningful if the target device has been seen during an inquiry. This can be by checking the result of -getLastInquiryUpdate. If nil is returned, then the device hasn’t been seen.

