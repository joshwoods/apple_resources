

- IOBluetooth
-  IOBluetoothIgnoreHIDDevice(\_:) 

Function

# IOBluetoothIgnoreHIDDevice(\_:)

Hints that the macOS Bluetooth software should ignore a HID device that connects up.

macOS

``` source
func IOBluetoothIgnoreHIDDevice(_ device: IOBluetoothDeviceRef!)
```

## Parameters 

`device`  

A Bluetooth Device to ignore.

## See Also

### Miscellaneous

func IOBluetoothL2CAPChannelRegisterForChannelCloseNotification(IOBluetoothL2CAPChannelRef!, IOBluetoothUserNotificationCallback!, UnsafeMutableRawPointer!) -> Unmanaged&lt;IOBluetoothUserNotificationRef>!

Allows a client to register for a channel close notification.

func IOBluetoothRemoveIgnoredHIDDevice(IOBluetoothDeviceRef!)

The counterpart to the above IOBluetoothIgnoreHIDDevice() API.

func IOBluetoothUserNotificationUnregister(IOBluetoothUserNotificationRef!)

Unregisters the target notification.

