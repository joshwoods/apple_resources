

- Kernel
- IOKit Fundamentals
- IOVideoDeviceNotificationMessage
-  mNotifications 

Instance Property

# mNotifications

A variable length array of IOVideoNotification structures that carry the actual notification data. The number of elements in this array is denoted by mNumberNotifications, but can also be inferred from the message size in the mach message header.

macOS 10.7+

``` source
IOVideoDeviceNotification mNotifications[1];
```

## See Also

### Fields

mMessageHeader

The mach message header.

mClientData

The client data that was registered with the mach port.

mNumberNotifications

The number of IOVideoNotifications in the mNotifications array.

