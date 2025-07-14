

- IOBluetooth
- IOBluetoothDeviceInquiryDelegate
-  deviceInquiryStarted(\_:) 

Instance Method

# deviceInquiryStarted(\_:)

macOS

``` source
optional func deviceInquiryStarted(_ sender: IOBluetoothDeviceInquiry!)
```

## Parameters 

`sender`  

Inquiry object that sent this delegate message.

## Discussion

This message will be delivered when the inquiry actually starts. Since the inquiry could be throttled, this message may not be received immediately after called -start.

