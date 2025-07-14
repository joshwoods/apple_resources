

- IOBluetooth UI
- IOBluetoothDeviceSelectorController
-  deviceSelector() 

Type Method

# deviceSelector()

macOS 10.2+

``` source
@MainActor
class func deviceSelector() -> IOBluetoothDeviceSelectorController!
```

## Return Value

Success - a new instance of the device selector Controller Failure - nil

## Discussion

Method call to instantiate a new IOBluetoothDeviceSelectorController object.

