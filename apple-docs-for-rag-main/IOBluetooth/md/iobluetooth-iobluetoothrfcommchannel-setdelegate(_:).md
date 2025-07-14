

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  setDelegate(\_:) 

Instance Method

# setDelegate(\_:)

Allows an object to register itself as a client of the RFCOMM channel.

macOS

``` source
func setDelegate(_ delegate: Any!) -> IOReturn
```

## Parameters 

`delegate`  

The object that will play the role of channel delegate \[NOTE the rfcomm channel will reatin the delegate\].

## Return Value

Returns kIOReturnSuccess if the delegate is successfully registered.

## Discussion

A channel delegate is the object the RFCOMM channel uses as target for data and events. The developer will implement only the the methods he/she is interested in. A list of the possible methods is at the end of this file in the definition of the informal protocol IOBluetoothRFCOMMChannelDelegate.

NOTE: This method is only available in macOS 10.2.5 (Bluetooth v1.2) or later. NOTE: Before OS X 10.6, the delegate was retained. On 10.6 and later, it is not.

