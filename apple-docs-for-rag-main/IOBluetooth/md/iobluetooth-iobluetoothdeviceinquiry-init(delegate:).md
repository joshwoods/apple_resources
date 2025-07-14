

- IOBluetooth
- IOBluetoothDeviceInquiry
-  init(delegate:) 

Initializer

# init(delegate:)

Initializes an alloc’d inquiry object, and sets the delegate object, as if -setDelegate: were called on it.

macOS

``` source
init!(delegate: Any!)
```

## Parameters 

`delegate`  

A delegate object that wishes to receive messages from the inquiry object. Delegate methods are listed below, under IOBluetoothDeviceInquiryDelegate.

## Return Value

A pointer to the initialized IOBluetoothDeviceInquiry object.

