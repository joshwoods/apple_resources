

- Exposure Notification
- ENStatus
-  ENStatus.restricted 

Case

# ENStatus.restricted

Notification is not active due to system restrictions, such as parental controls.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
case restricted
```

## Discussion

When in this state, the app cannot enable exposure notification.

## See Also

### States

case active

Notification is active.

case bluetoothOff

Bluetooth is turned off.

case disabled

Notification is disabled.

case unknown

Notification is unknown.

case paused

The user paused Exposure Notification.

case unauthorized

The user hasn’t authorized Exposure Notification.

