

- IOBluetooth
- IOBluetoothDeviceInquiryDelegate
-  deviceInquiryComplete(\_:error:aborted:) 

Instance Method

# deviceInquiryComplete(\_:error:aborted:)

macOS

``` source
optional func deviceInquiryComplete(
    _ sender: IOBluetoothDeviceInquiry!,
    error: IOReturn,
    aborted: Bool
)
```

## Parameters 

`sender`  

Inquiry object that sent this delegate message.

`error`  

Error code. kIOReturnSuccess if the inquiry completed without incident.

`aborted`  

TRUE if user called -stop on the inquiry.

## Discussion

When the inquiry is completely stopped, this delegate method will be invoked. It will supply an error code value, kIOReturnSuccess if the inquiry stopped without problem, otherwise a non-kIOReturnSuccess error code will be supplied.

