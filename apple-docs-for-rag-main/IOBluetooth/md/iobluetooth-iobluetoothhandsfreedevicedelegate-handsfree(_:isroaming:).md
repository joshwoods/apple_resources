

- IOBluetooth
- IOBluetoothHandsFreeDeviceDelegate
-  handsFree(\_:isRoaming:) 

Instance Method

# handsFree(\_:isRoaming:)

Tells the delegate the roaming indicator of the connected Bluetooth hands-free phone or headset has changed.

macOS 10.7+

``` source
optional func handsFree(
    _ device: IOBluetoothHandsFreeDevice!,
    isRoaming: NSNumber!
)
```

## Parameters 

`device`  

The connected Bluetooth hands-free phone or headset.

`isRoaming`  

The new value of the roaming indicator. For possible values, see IOBluetoothHandsFreeIndicatorRoam.

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

func handsFree(IOBluetoothHandsFreeDevice!, batteryCharge: NSNumber!)

Tells the delegate the battery level indicator of the connected Bluetooth hands-free phone or headset has changed.

