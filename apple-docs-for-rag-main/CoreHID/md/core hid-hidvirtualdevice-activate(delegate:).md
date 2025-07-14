

- Core HID
- HIDVirtualDevice
-  activate(delegate:) 

Instance Method

# activate(delegate:)

Activate a newly created virtual device to begin receiving notifications and enable functionality.

macOS 15.0+

``` source
func activate(delegate: any HIDVirtualDeviceDelegate)
```

## Parameters 

`delegate`  

The HIDVirtualDeviceDelegate that receives incoming set/get report requests. Only one delegate is associated with the device, but many devices can be associated with the delegate.

## Discussion

Many functions won’t run, and notifications won’t be received using the HIDVirtualDeviceDelegate until activate has run successfully. A device cannot be activated twice.

## See Also

### Create a HID virtual device

init?(properties: HIDVirtualDevice.Properties)

Creates a virtual HID device.

let deviceReference: HIDDeviceClient.DeviceReference

The reference to the virtual HID device.

