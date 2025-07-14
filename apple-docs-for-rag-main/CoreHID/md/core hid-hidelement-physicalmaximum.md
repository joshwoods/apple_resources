

- Core HID
- HIDElement
-  physicalMaximum 

Instance Property

# physicalMaximum

The physical maximum for this element’s data.

macOS 15.0+

``` source
var physicalMaximum: Int64?
```

## Discussion

The physical maximum combines with the physical minimum to determine the shifting and scaling required to transform the raw report data into the actual value that has meaning for the device.

See the HID specification for more details: https://www.usb.org/hid.

