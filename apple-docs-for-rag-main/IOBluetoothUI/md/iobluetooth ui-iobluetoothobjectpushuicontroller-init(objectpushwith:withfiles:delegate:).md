

- IOBluetooth UI
- IOBluetoothObjectPushUIController
-  init(objectPushWith:withFiles:delegate:) 

Initializer

# init(objectPushWith:withFiles:delegate:)

Creates and returns a new IOBluetoothObjectPush object

macOS 10.2+

``` source
@MainActor
init!(
    objectPushWith inDevice: IOBluetoothDevice!,
    withFiles inFiles: [Any]!,
    delegate inDelegate: Any!
)
```

## Parameters 

`inDevice`  

The remote device to send the files to

`inFiles`  

An array of file paths to send

`inDelegate`  

A delegate object that implements the single method above. If no delegate is specified this object will release itself when the transaction is complete.

## Discussion

The event delegate should implement a single delegate method:

- (void) objectPushComplete: (IOBluetoothObjectPushUIController\*) inPusher

The method will be called when the transaction is complete and should be used to release the push object by the delegate. If no delegate is set the object will release itself when the transfer is finished.

