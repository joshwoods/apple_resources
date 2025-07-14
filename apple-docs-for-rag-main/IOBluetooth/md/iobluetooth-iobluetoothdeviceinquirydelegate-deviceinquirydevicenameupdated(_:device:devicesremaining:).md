

- IOBluetooth
- IOBluetoothDeviceInquiryDelegate
-  deviceInquiryDeviceNameUpdated(\_:device:devicesRemaining:) 

Instance Method

# deviceInquiryDeviceNameUpdated(\_:device:devicesRemaining:)

macOS

``` source
optional func deviceInquiryDeviceNameUpdated(
    _ sender: IOBluetoothDeviceInquiry!,
    device: IOBluetoothDevice!,
    devicesRemaining: UInt32
)
```

## Parameters 

`sender`  

Inquiry object that sent this delegate message.

`device`  

IOBluetoothDevice that was updated.

`devicesRemaining`  

Number of devices remaining to update.

## Discussion

A device name has been retrieved. Also indicates how many devices are left to be updated.

