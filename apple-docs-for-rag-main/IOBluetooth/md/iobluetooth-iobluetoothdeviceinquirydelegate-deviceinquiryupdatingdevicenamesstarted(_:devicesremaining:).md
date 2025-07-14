

- IOBluetooth
- IOBluetoothDeviceInquiryDelegate
-  deviceInquiryUpdatingDeviceNamesStarted(\_:devicesRemaining:) 

Instance Method

# deviceInquiryUpdatingDeviceNamesStarted(\_:devicesRemaining:)

macOS

``` source
optional func deviceInquiryUpdatingDeviceNamesStarted(
    _ sender: IOBluetoothDeviceInquiry!,
    devicesRemaining: UInt32
)
```

## Parameters 

`sender`  

Inquiry object that sent this delegate message.

`devicesRemaining`  

Number of devices remaining to update.

## Discussion

The inquiry has begun updating device names that were found during the search.

