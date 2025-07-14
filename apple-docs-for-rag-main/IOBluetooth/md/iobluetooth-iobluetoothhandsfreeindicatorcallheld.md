

- IOBluetooth
-  IOBluetoothHandsFreeIndicatorCallHeld 

Global Variable

# IOBluetoothHandsFreeIndicatorCallHeld

The command string you use to show a call hold status indicator on a phone.

macOS

``` source
let IOBluetoothHandsFreeIndicatorCallHeld: String
```

## Discussion

The possible values for the hold indicator are:

`0`  
No calls are on hold.

`1`  
A call is on hold and another is active.

`2`  
A call is on hold and no calls are active.

## See Also

### Call Status

let IOBluetoothHandsFreeIndicatorCall: String

The command string you use to show an active call indicator on a phone.

let IOBluetoothHandsFreeIndicatorCallSetup: String

The command string you use to show a call setup status indicator on a phone.

