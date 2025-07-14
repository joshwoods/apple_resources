

- IOBluetooth
- IOBluetoothDevice
-  getLastInquiryUpdate() 

Instance Method

# getLastInquiryUpdate()

Get the date/time of the last time the device was returned during an inquiry.

macOS

``` source
func getLastInquiryUpdate() -> Date!
```

## Return Value

Returns the date/time of the last time the device was seen during an inquiry. If the device has never been seen during an inquiry, nil is returned.

