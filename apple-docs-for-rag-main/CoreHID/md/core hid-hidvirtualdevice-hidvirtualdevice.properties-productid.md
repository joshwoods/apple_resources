

- Core HID
- HIDVirtualDevice
- HIDVirtualDevice.Properties
-  productID 

Instance Property

# productID

The product ID for the device.

macOS 15.0+

``` source
let productID: UInt32?
```

## Discussion

The product ID combines with vendorID to specify the exact product. Without knowing the vendor, product ID is useless. Look for vendor specific documentation for more details on the assigned product IDs for their products.

