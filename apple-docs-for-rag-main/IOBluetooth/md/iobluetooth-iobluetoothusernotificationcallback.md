

- IOBluetooth
-  IOBluetoothUserNotificationCallback 

Type Alias

# IOBluetoothUserNotificationCallback

Callback function definition for user notifications.

macOS

``` source
typealias IOBluetoothUserNotificationCallback = (UnsafeMutableRawPointer?, IOBluetoothUserNotificationRef?, IOBluetoothObjectRef?) -> Void
```

## Parameters 

`userRefCon`  

(Void \*) This user defined parameter was provided during the original call to register the notification.

`inRef`  

(IOBluetoothUserNotificationRef) The notification responsible for sending the notification.

`status`  

(IOBluetoothObjectRef) The object that originated the notification.

## Return Value

None.

## Discussion

This callback will be invoked when the notification for which it was registered is sent.

