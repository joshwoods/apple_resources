

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  handsFree(\_:incomingCallFrom:) 

Instance Method

# handsFree(\_:incomingCallFrom:)

Tells the delegate there’s an incoming call on the connected Bluetooth hands-free phone or headset.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeDevice!,
    incomingCallFrom number: String!
)
```

## Parameters 

`device`  

The connected Bluetooth hands-free phone or headset.

`number`  

The phone number of the caller.

## See Also

### Receiving Call Status

func handsFree(IOBluetoothHandsFreeDevice!, currentCall: [AnyHashable : Any]!)

Sends the delegate information about the current call.

Current Call Information Constants

Get information about a phone call on a hands-free Bluetooth device.

