

- IOBluetooth
- IOBluetoothHandsFree
-  deviceSupportedFeatures 

Instance Property

# deviceSupportedFeatures

Return the device’s supported features.

macOS 10.7+

``` source
var deviceSupportedFeatures: UInt32 { get }
```

## Return Value

The device features bitmap

## Discussion

Returns the device’s supported features bitmap. The values are described in “IOBluetoothHandsFreeDeviceFeatures and IOBluetoothHandsFreeAudioGatewayFeatures.”

