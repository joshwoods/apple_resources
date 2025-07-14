

- Core HID
- HIDElement
-  physicalMinimum 

Instance Property

# physicalMinimum

The physical minimum for this element’s data.

macOS 15.0+

``` source
var physicalMinimum: Int64?
```

## Discussion

The physical minimum combines with the physical maximum to determine the shifting and scaling required to transform the raw report data into the actual value that has meaning for the device.

See the HID specification for more details: https://www.usb.org/hid.

