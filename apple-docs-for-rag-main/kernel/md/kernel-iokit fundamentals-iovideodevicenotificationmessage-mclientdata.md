

- Kernel
- IOKit Fundamentals
- IOVideoDeviceNotificationMessage
-  mClientData 

Instance Property

# mClientData

The client data that was registered with the mach port.

macOS 10.7+

``` source
UInt32 mClientData;
```

## See Also

### Fields

mMessageHeader

The mach message header.

mNumberNotifications

The number of IOVideoNotifications in the mNotifications array.

mNotifications

A variable length array of IOVideoNotification structures that carry the actual notification data. The number of elements in this array is denoted by mNumberNotifications, but can also be inferred from the message size in the mach message header.

