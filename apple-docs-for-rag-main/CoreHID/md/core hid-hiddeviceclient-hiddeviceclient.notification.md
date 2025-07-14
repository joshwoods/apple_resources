

- Core HID
- HIDDeviceClient
-  HIDDeviceClient.Notification 

Enumeration

# HIDDeviceClient.Notification

Notifications for a HID device.

macOS 15.0+

``` source
enum Notification
```

## Overview

You can receive these notifications using monitorNotifications(reportIDsToMonitor:elementsToMonitor:).

## Topics

### Enumeration Cases

case deviceRemoved

A notification that the device is no longer connected to the system.

case deviceSeized

A notification that the device was seized by another client.

case deviceUnseized

A notification that the device is no longer seized.

case elementUpdates(values: [HIDElement.Value])

A notification that elements of the device were updated.

case inputReport(id: HIDReportID?, data: Data, timestamp: SuspendingClock.Instant)

A notification that an input report was received from the device.

## Relationships

### Conforms To

- Sendable

## See Also

### Monitor device notifications

func monitorNotifications(reportIDsToMonitor: [ClosedRange&lt;HIDReportID>], elementsToMonitor: [HIDElement]) -> AsyncThrowingStream&lt;HIDDeviceClient.Notification, any Error>

Creates an asynchronous that receives notifications about the associated device.

