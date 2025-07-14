

- IOBluetooth
- IOBluetoothHandsFreeAudioGateway
-  Status Indicator Constants 

API Collection

# Status Indicator Constants

Send commands to modify the status indicators of a hands-free Bluetooth device.

## Topics

### Call Status

let IOBluetoothHandsFreeIndicatorCall: String

The command string you use to show an active call indicator on a phone.

let IOBluetoothHandsFreeIndicatorCallHeld: String

The command string you use to show a call hold status indicator on a phone.

let IOBluetoothHandsFreeIndicatorCallSetup: String

The command string you use to show a call setup status indicator on a phone.

### Phone Network Connection

let IOBluetoothHandsFreeIndicatorRoam: String

The command string you use to show a roaming status indicator on a phone.

let IOBluetoothHandsFreeIndicatorSignal: String

The command string you use to show a signal strength indicator on a phone.

let IOBluetoothHandsFreeIndicatorService: String

The command string you use to show a carrier network connection indicator on a phone.

### Phone Status

let IOBluetoothHandsFreeIndicatorBattChg: String

The command string you use to show a battery charge level indicator on a phone.

## See Also

### Showing Status Indicators

func createIndicator(String!, min: Int32, max: Int32, currentValue: Int32)

Sends a request to the Bluetooth device to show or update a status indicator.

