

- IOBluetooth
-  IOBluetoothHandsFreeCallIndex 

Global Variable

# IOBluetoothHandsFreeCallIndex

The index of the call, starting with `1`.

macOS

``` source
let IOBluetoothHandsFreeCallIndex: String
```

## Discussion

Calls keep their index number until they are ended. New calls are assigned the lowest available index number.

## See Also

### Call Information

let IOBluetoothHandsFreeCallDirection: String

A value that indicates whether a call is incoming or outgoing.

let IOBluetoothHandsFreeCallMode: String

The type of call data.

let IOBluetoothHandsFreeCallMultiparty: String

A value that indicates whether the call is multiple-party.

let IOBluetoothHandsFreeCallStatus: String

The current state of the call.

