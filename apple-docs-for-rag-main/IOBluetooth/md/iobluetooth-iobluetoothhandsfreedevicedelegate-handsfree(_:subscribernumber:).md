

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  handsFree(\_:subscriberNumber:) 

Instance Method

# handsFree(\_:subscriberNumber:)

Tells the delegate the subscriber number of a call.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeDevice!,
    subscriberNumber: String!
)
```

## Parameters 

`device`  

The connected Bluetooth hands-free phone or headset.

`subscriberNumber`  

The subscriber number.

## Discussion

If multiple subscriber numbers are on the gateway, this function is called once for each subscriber number.

## See Also

### Receiving Other Information

func handsFree(IOBluetoothHandsFreeDevice!, ringAttempt: NSNumber!)

Tells the delegate the phone is ringing.

func handsFree(IOBluetoothHandsFreeDevice!, unhandledResultCode: String!)

Tells the delegate the phone sent an unknown code.

