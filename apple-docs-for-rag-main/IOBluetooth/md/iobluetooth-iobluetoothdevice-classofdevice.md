

- IOBluetooth
- IOBluetoothDevice
-  classOfDevice 

Instance Property

# classOfDevice

Gets the full class of device value for the remote device.

macOS

``` source
var classOfDevice: BluetoothClassOfDevice { get }
```

## Discussion

This value is only meaningful if the target device has been seen during an inquiry. This can be by checking the result of -getLastInquiryUpdate. If nil is returned, then the device hasn’t been seen.

