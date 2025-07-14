

- Core HID
- HIDElement
-  logicalMinimum 

Instance Property

# logicalMinimum

The logical minimum for this element’s data.

macOS 15.0+

``` source
var logicalMinimum: Int64?
```

## Discussion

The logical minimum is specified in the report descriptor for an element. It determines the minimum raw value that should be considered valid, anything below this value is invalid.

See the HID specification for more details: https://www.usb.org/hid.

