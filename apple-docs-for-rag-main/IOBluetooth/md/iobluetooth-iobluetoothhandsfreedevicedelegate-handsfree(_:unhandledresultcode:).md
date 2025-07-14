

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  handsFree(\_:unhandledResultCode:) 

Instance Method

# handsFree(\_:unhandledResultCode:)

Tells the delegate the phone sent an unknown code.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeDevice!,
    unhandledResultCode resultCode: String!
)
```

## Parameters 

`device`  

The connected Bluetooth hands-free phone or headset.

`resultCode`  

A string containing the result code. The `“/r/n”` strings are stripped from the beginning and end.

## See Also

### Receiving Other Information

func handsFree(IOBluetoothHandsFreeDevice!, subscriberNumber: String!)

Tells the delegate the subscriber number of a call.

func handsFree(IOBluetoothHandsFreeDevice!, ringAttempt: NSNumber!)

Tells the delegate the phone is ringing.

