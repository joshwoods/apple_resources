

- Core HID
- HIDDeviceClient
- HIDDeviceClient.RequestElementUpdate
-  init(elements:pollDevice:) 

Initializer

# init(elements:pollDevice:)

Creates a request element update.

macOS 15.0+

``` source
init(
    elements: [HIDElement],
    pollDevice: Bool = true
)
```

## Parameters 

`elements`  

The elements used to request updates.

`pollDevice`  

Whether the device should be polled for new updates, or if the most recently received values can be returned without device interaction. If true, one or more get report requests are issued to the device.

