

- IOBluetooth
- IOBluetoothL2CAPChannel
-  incomingMTU 

Instance Property

# incomingMTU

Returns the current incoming MTU for the L2CAP channel.

macOS

``` source
var incomingMTU: BluetoothL2CAPMTU { get }
```

## Discussion

The incoming MTU represents the maximum L2CAP packet size for packets being sent by the remote device.

