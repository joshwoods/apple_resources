

- IOBluetooth
-  IOBluetoothRemoveIgnoredHIDDevice(\_:) 

Function

# IOBluetoothRemoveIgnoredHIDDevice(\_:)

The counterpart to the above IOBluetoothIgnoreHIDDevice() API.

macOS

``` source
func IOBluetoothRemoveIgnoredHIDDevice(_ device: IOBluetoothDeviceRef!)
```

## Parameters 

`device`  

A Bluetooth Device to “un”ignore.

## See Also

### Miscellaneous

func IOBluetoothIgnoreHIDDevice(IOBluetoothDeviceRef!)

Hints that the macOS Bluetooth software should ignore a HID device that connects up.

func IOBluetoothL2CAPChannelRegisterForChannelCloseNotification(IOBluetoothL2CAPChannelRef!, IOBluetoothUserNotificationCallback!, UnsafeMutableRawPointer!) -> Unmanaged&lt;IOBluetoothUserNotificationRef>!

Allows a client to register for a channel close notification.

func IOBluetoothUserNotificationUnregister(IOBluetoothUserNotificationRef!)

Unregisters the target notification.

