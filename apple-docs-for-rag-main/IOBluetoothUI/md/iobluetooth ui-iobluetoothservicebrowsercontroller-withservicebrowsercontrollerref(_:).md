

- IOBluetooth UI
- IOBluetoothServiceBrowserController
-  withServiceBrowserControllerRef(\_:) 

Type Method

# withServiceBrowserControllerRef(\_:)

Method call to convert an IOBluetoothServiceBrowserControllerRef into an IOBluetoothServiceBrowserController \*.

macOS 10.2+

``` source
@MainActor
class func withServiceBrowserControllerRef(_ serviceBrowserControllerRef: IOBluetoothServiceBrowserControllerRef!) -> IOBluetoothServiceBrowserController!
```

## Parameters 

`serviceBrowserControllerRef`  

IOBluetoothServiceBrowserControllerRef for which an IOBluetoothServiceBrowserController \* is desired.

## Return Value

Returns the IOBluetoothServiceBrowserController \* for the given IOBluetoothServiceBrowserControllerRef.

