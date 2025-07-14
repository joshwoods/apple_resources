

- Core HID
- HIDDeviceManager
- HIDDeviceManager.DeviceMatchingCriteria
-  productID 

Instance Property

# productID

The product ID for the device.

macOS 15.0+

``` source
var productID: UInt32?
```

## Discussion

The product ID combines with the vendorID to specify the exact product. Without knowing the vendor, the product ID is meaningless. Look for vendor specific documentation for more details on the assigned product IDs for a vendor’s products.

