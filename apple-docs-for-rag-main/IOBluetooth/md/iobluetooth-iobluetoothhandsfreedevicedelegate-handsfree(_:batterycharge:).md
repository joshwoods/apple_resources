

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  handsFree(\_:batteryCharge:) 

Instance Method

# handsFree(\_:batteryCharge:)

Tells the delegate the battery level indicator of the connected Bluetooth hands-free phone or headset has changed.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeDevice!,
    batteryCharge: NSNumber!
)
```

## Parameters 

`device`  

The connected Bluetooth hands-free phone or headset.

`batteryCharge`  

The new value of the battery level indicator. For possible values, see IOBluetoothHandsFreeIndicatorBattChg.

## See Also

### Receiving Status Indicator Changes

func handsFree(IOBluetoothHandsFreeDevice!, callSetupMode: NSNumber!)

Tells the delegate the call setup indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, isCallActive: NSNumber!)

Tells the delegate the active call indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, isServiceAvailable: NSNumber!)

Tells the delegate the service level indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, signalStrength: NSNumber!)

Tells the delegate the call setup signal strength indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, callHoldState: NSNumber!)

Tells the delegate the call held indicator of the connected Bluetooth hands-free phone or headset has changed.

func handsFree(IOBluetoothHandsFreeDevice!, isRoaming: NSNumber!)

Tells the delegate the roaming indicator of the connected Bluetooth hands-free phone or headset has changed.

