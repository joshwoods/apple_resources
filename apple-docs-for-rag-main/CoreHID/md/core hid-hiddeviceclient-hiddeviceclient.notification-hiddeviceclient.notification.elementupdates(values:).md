

- Core HID
- HIDDeviceClient
- HIDDeviceClient.Notification
-  HIDDeviceClient.Notification.elementUpdates(values:) 

Case

# HIDDeviceClient.Notification.elementUpdates(values:)

A notification that elements of the device were updated.

macOS 15.0+

``` source
case elementUpdates(values: [HIDElement.Value])
```

## Parameters 

`values`  

The updated values.

## Mentioned in 

Communicating with human interface devices

## Discussion

This is typically received in response to input reports, and is another way to receive the data in a different format than HIDDeviceClient.Notification.inputReport(id:data:timestamp:).

