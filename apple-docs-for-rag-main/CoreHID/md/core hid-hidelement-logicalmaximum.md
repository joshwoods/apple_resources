

- Core HID
- HIDElement
-  logicalMaximum 

Instance Property

# logicalMaximum

The logical maximum for this element’s data.

macOS 15.0+

``` source
var logicalMaximum: Int64?
```

## Discussion

The logical maximum is specified in the report descriptor for an element. It determines the maximum raw value that should be considered valid, anything above this value is invalid.

See the HID specification for more details: https://www.usb.org/hid.

