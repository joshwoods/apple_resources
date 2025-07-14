

- Kernel
- IOKit Fundamentals
- IOVideoDeviceNotificationMessage
-  mNumberNotifications 

Instance Property

# mNumberNotifications

The number of IOVideoNotifications in the mNotifications array.

macOS 10.7+

``` source
UInt32 mNumberNotifications;
```

## See Also

### Fields

mMessageHeader

The mach message header.

mClientData

The client data that was registered with the mach port.

mNotifications

A variable length array of IOVideoNotification structures that carry the actual notification data. The number of elements in this array is denoted by mNumberNotifications, but can also be inferred from the message size in the mach message header.

