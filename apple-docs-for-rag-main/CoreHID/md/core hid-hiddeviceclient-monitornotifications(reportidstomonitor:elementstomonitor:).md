

- Core HID
- HIDDeviceClient
-  monitorNotifications(reportIDsToMonitor:elementsToMonitor:) 

Instance Method

# monitorNotifications(reportIDsToMonitor:elementsToMonitor:)

Creates an asynchronous that receives notifications about the associated device.

macOS 15.0+

``` source
func monitorNotifications(
    reportIDsToMonitor: [ClosedRange],
    elementsToMonitor: [HIDElement]
) -> AsyncThrowingStream
```

## Parameters 

`reportIDsToMonitor`  

The report IDs that should trigger an HIDDeviceClient.Notification.inputReport(id:data:timestamp:) notification.

`elementsToMonitor`  

The elements that should trigger an HIDDeviceClient.Notification.elementUpdates(values:) notification. Elements of interest can be parsed from elements.

## Return Value

An asynchronous stream that receive notifications.

## Mentioned in 

Communicating with human interface devices

## Discussion

Notifications come in asynchronously from the device at arbitrary times when relevant events occur.

Example usage:

```
for await notification in try await client.monitorNotifications(reportIDsToMonitor: [HIDReportID.allReports], elementsToMonitor: await client.elements) {
switch notification {
case .inputReport(let reportID, let report, let timestamp):
    break
case .elementUpdates(let values):
    break
case .deviceSeized:
    break
case .deviceUnseized:
    break
case .deviceRemoved:
    break
}
```

Throws

HIDDeviceError if there is an issue with setup.

## See Also

### Monitor device notifications

enum Notification

Notifications for a HID device.

