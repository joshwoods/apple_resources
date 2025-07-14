

- IOBluetooth
-  IOBluetoothHandsFreeIndicatorCallSetup 

Global Variable

# IOBluetoothHandsFreeIndicatorCallSetup

The command string you use to show a call setup status indicator on a phone.

macOS

``` source
let IOBluetoothHandsFreeIndicatorCallSetup: String
```

## Discussion

The possible values for the call setup indicator are:

`0`  
No calls are being set up.

`1`  
An incoming call is being set up.

`2`  
An outgoing call is being set up.

`3`  
The party receiving the call is being notified.

## See Also

### Call Status

let IOBluetoothHandsFreeIndicatorCall: String

The command string you use to show an active call indicator on a phone.

let IOBluetoothHandsFreeIndicatorCallHeld: String

The command string you use to show a call hold status indicator on a phone.

