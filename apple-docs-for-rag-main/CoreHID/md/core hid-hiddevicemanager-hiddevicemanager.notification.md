

- Core HID
- HIDDeviceManager
-  HIDDeviceManager.Notification 

Enumeration

# HIDDeviceManager.Notification

Notifications for HID devices.

macOS 15.0+

``` source
enum Notification
```

## Overview

You can receive these notifications using monitorNotifications(matchingCriteria:).

## Topics

### Enumeration Cases

case deviceMatched(HIDDeviceClient.DeviceReference)

A notification that a device matched the device criteria.

case deviceRemoved(HIDDeviceClient.DeviceReference)

A notification that a previously matched device was removed from the system.

## Relationships

### Conforms To

- Sendable

## See Also

### Monitor device notifications

func monitorNotifications(matchingCriteria: [HIDDeviceManager.DeviceMatchingCriteria]) -> AsyncThrowingStream&lt;HIDDeviceManager.Notification, any Error>

Creates an asynchronous stream that receives notifications for devices of interest.

