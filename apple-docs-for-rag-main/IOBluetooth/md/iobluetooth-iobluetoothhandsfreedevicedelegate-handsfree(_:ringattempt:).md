

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  handsFree(\_:ringAttempt:) 

Instance Method

# handsFree(\_:ringAttempt:)

Tells the delegate the phone is ringing.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeDevice!,
    ringAttempt: NSNumber!
)
```

## Parameters 

`device`  

The connected Bluetooth hands-free phone or headset.

`ringAttempt`  

The number of ring alerts received for the call.

## See Also

### Receiving Other Information

func handsFree(IOBluetoothHandsFreeDevice!, subscriberNumber: String!)

Tells the delegate the subscriber number of a call.

func handsFree(IOBluetoothHandsFreeDevice!, unhandledResultCode: String!)

Tells the delegate the phone sent an unknown code.

