

- IOBluetooth
- IOBluetoothHandsFree
-  init(device:delegate:) 

Initializer

# init(device:delegate:)

Create a new IOBluetoothHandsFree object

macOS 10.7+

``` source
init!(
    device: IOBluetoothDevice!,
    delegate inDelegate: (any IOBluetoothHandsFreeDelegate)!
)
```

## Parameters 

`device`  

An IOBluetoothDevice

`inDelegate`  

An object to act as delegate that implements the IOBluetoothHandsFreeDelegate protocol.

## Return Value

A newly created IOBluetoothHandsFreeAudioGateway object on success, nil on failure

## Discussion

This method should be called on a subclass (IOBluetoothHandsFreeDevice or IOBluetoothHandsFreeAudioGateway) to get full functionality.

