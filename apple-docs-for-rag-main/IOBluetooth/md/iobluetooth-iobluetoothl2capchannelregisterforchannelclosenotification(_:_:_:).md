

- IOBluetooth
-  IOBluetoothL2CAPChannelRegisterForChannelCloseNotification(\_:\_:\_:) 

Function

# IOBluetoothL2CAPChannelRegisterForChannelCloseNotification(\_:\_:\_:)

Allows a client to register for a channel close notification.

macOS

``` source
func IOBluetoothL2CAPChannelRegisterForChannelCloseNotification(
    _ channel: IOBluetoothL2CAPChannelRef!,
    _ callback: IOBluetoothUserNotificationCallback!,
    _ inRefCon: UnsafeMutableRawPointer!
) -> Unmanaged!
```

## Parameters 

`channel`  

The target L2CAP channel

`callback`  

Callback to be called when the L2CAP channel is closed.

`inRefCon`  

Client-supplied refCon to be passed to the callback.

## Return Value

Returns an IOBluetoothUserNotificationRef representing the outstanding L2CAP channel close notification. To unregister the notification, call IOBluetoothUserNotificationUnregister() with the returned IOBluetoothUserNotificationRef. If an error is encountered creating the notification, NULL is returned. The returned IOBluetoothUserNotificationRef will be valid for as long as the notification is registered. It is not necessary to retain the result. Once the notification is unregistered, it will no longer be valid.

## Discussion

The given callback will be called when the L2CAP channel is closed.

## See Also

### Miscellaneous

func IOBluetoothIgnoreHIDDevice(IOBluetoothDeviceRef!)

Hints that the macOS Bluetooth software should ignore a HID device that connects up.

func IOBluetoothRemoveIgnoredHIDDevice(IOBluetoothDeviceRef!)

The counterpart to the above IOBluetoothIgnoreHIDDevice() API.

func IOBluetoothUserNotificationUnregister(IOBluetoothUserNotificationRef!)

Unregisters the target notification.

