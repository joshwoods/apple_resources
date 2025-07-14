

- Exposure Notification
- ENStatus
-  ENStatus.disabled 

Case

# ENStatus.disabled

Notification is disabled.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
case disabled
```

## Discussion

Use setExposureNotificationEnabled(_:completionHandler:) to enable exposure notification.

## See Also

### States

case active

Notification is active.

case bluetoothOff

Bluetooth is turned off.

case restricted

Notification is not active due to system restrictions, such as parental controls.

case unknown

Notification is unknown.

case paused

The user paused Exposure Notification.

case unauthorized

The user hasn’t authorized Exposure Notification.

