

- IOBluetooth
- IOBluetoothDeviceInquiryDelegate
-  deviceInquiryDeviceFound(\_:device:) 

Instance Method

# deviceInquiryDeviceFound(\_:device:)

macOS

``` source
optional func deviceInquiryDeviceFound(
    _ sender: IOBluetoothDeviceInquiry!,
    device: IOBluetoothDevice!
)
```

## Parameters 

`sender`  

Inquiry object that sent this delegate message.

`device`  

IOBluetoothDevice that was found.

## Discussion

A new device has been found. You do not need to retain the device - it will be held in the internal storage of the inquiry, and can be accessed later using -foundDevices.

