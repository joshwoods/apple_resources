

- IOBluetooth UI
- IOBluetoothServiceBrowserController
-  init(\_:) 

Initializer

# init(\_:)

Allocator work Bluetooth Service Browser window controller.

macOS 10.2+

``` source
@MainActor
init!(_ inOptions: IOBluetoothServiceBrowserControllerOptions)
```

## Parameters 

`inOptions`  

Bit field for options to set in the newly allocated controller. Currently no options are available.

## Return Value

A new instance of the IOBluetoothServiceBrowserController Controller, nil if unsuccessful.

