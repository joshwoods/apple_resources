

- Core HID
- HIDVirtualDevice
- HIDVirtualDevice.Properties
-  descriptor 

Instance Property

# descriptor

The HID specification compliant report descriptor for the virtual device.

macOS 15.0+

``` source
let descriptor: Data
```

## Mentioned in 

Creating virtual devices

## Discussion

A report descriptor defines details about the device and the type of interactions that it can have, such as the type of input it can generate, and the queries it responds to. This is the raw descriptor in byte form.

For more details, see Human Interface Devices (HID) Specifications and Tools.

