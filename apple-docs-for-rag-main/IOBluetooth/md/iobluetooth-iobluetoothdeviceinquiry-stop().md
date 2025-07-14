

- IOBluetooth
- IOBluetoothDeviceInquiry
-  stop() 

Instance Method

# stop()

Halts the inquiry object. Could either stop the search for new devices, or the updating of found device names.

macOS

``` source
func stop() -> IOReturn
```

## Return Value

Returns kIOReturnSuccess if the inquiry is successfully stopped. Returns kIOReturnNotPermitted if the inquiry object is already stopped. May return other IOReturn values, as appropriate.

