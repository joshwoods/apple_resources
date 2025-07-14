

- Exposure Notification
- ENStatus
-  ENStatus.bluetoothOff 

Case

# ENStatus.bluetoothOff

Bluetooth is turned off.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
case bluetoothOff
```

## Discussion

Bluetooth is required for Exposure Notification. If Bluetooth is disabled, notify the user that Exposure Notification can’t work without Bluetooth enabled.

Note

This may not match the state of Bluetooth as reported by CoreBluetooth.

Exposure Notification is a system service and can use Bluetooth in situations when apps cannot. For the purposes of notification of exposure, it’s better to use this API instead of CoreBluetooth.

## See Also

### States

case active

Notification is active.

case disabled

Notification is disabled.

case restricted

Notification is not active due to system restrictions, such as parental controls.

case unknown

Notification is unknown.

case paused

The user paused Exposure Notification.

case unauthorized

The user hasn’t authorized Exposure Notification.

