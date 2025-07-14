

- IOBluetooth
- IOBluetoothL2CAPChannel
-  requestRemoteMTU(\_:) 

Instance Method

# requestRemoteMTU(\_:)

Initiates the process to reconfigure the L2CAP channel with a new outgoing MTU.

macOS

``` source
func requestRemoteMTU(_ remoteMTU: BluetoothL2CAPMTU) -> IOReturn
```

## Parameters 

`remoteMTU`  

The desired outgoing MTU.

## Return Value

Returns kIOReturnSuccess if the channel re-configure process was successfully initiated.

## Discussion

Currently, this API does not give an indication that the re-config process has completed. In the future additional API will be available to provide that information both synchronously and asynchronously.

