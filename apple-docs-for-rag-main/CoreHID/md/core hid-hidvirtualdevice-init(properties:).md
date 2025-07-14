

- Core HID
- HIDVirtualDevice
-  init(properties:) 

Initializer

# init(properties:)

Creates a virtual HID device.

macOS 15.0+

``` source
init?(properties: HIDVirtualDevice.Properties)
```

## Parameters 

`properties`  

The HIDVirtualDevice.Properties for the virtual device. These values determine the device functionality.

## Discussion

HIDVirtualDevice is created in an inactive state, notifications won’t be received and many functions won’t run until activate(delegate:) has run successfully.

## See Also

### Create a HID virtual device

let deviceReference: HIDDeviceClient.DeviceReference

The reference to the virtual HID device.

func activate(delegate: any HIDVirtualDeviceDelegate)

Activate a newly created virtual device to begin receiving notifications and enable functionality.

