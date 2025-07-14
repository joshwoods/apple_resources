

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  handsFree(\_:incomingSMS:) 

Instance Method

# handsFree(\_:incomingSMS:)

Tells the delegate there’s an incoming text message.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeDevice!,
    incomingSMS sms: [AnyHashable : Any]!
)
```

## Parameters 

`device`  

The connected Bluetooth hands-free phone or headset.

`sms`  

A dictionary containing the incoming SMS message. For dictionary keys, see SMS Dictionary Key Constants.

## See Also

### Receiving SMS Information

SMS Dictionary Key Constants

Read the parts of an SMS message.

