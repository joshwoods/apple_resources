

- IOBluetooth
- IOBluetoothDeviceInquiry
-  updateNewDeviceNames 

Instance Property

# updateNewDeviceNames

Sets whether or not the inquiry object will retrieve the names of devices found during the search.

macOS

``` source
var updateNewDeviceNames: Bool { get set }
```

## Parameters 

`inValue`  

Pass TRUE if names are to be updated, otherwise pass FALSE.

## Discussion

The default value for the inquiry object is TRUE, unless this method is used to change it.

