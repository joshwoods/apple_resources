

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  handsFree(\_:currentCall:) 

Instance Method

# handsFree(\_:currentCall:)

Sends the delegate information about the current call.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeDevice!,
    currentCall: [AnyHashable : Any]!
)
```

## Parameters 

`device`  

The connected Bluetooth hands-free phone or headset.

`currentCall`  

A dictionary with the incoming SMS message. For dictionary keys, see Current Call Information Constants.

## See Also

### Receiving Call Status

func handsFree(IOBluetoothHandsFreeDevice!, incomingCallFrom: String!)

Tells the delegate there’s an incoming call on the connected Bluetooth hands-free phone or headset.

Current Call Information Constants

Get information about a phone call on a hands-free Bluetooth device.

