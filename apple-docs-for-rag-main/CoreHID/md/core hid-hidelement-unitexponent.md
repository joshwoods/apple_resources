

- Core HID
- HIDElement
-  unitExponent 

Instance Property

# unitExponent

The calculated exponent for this element.

macOS 15.0+

``` source
var unitExponent: Int8?
```

## Discussion

Some items in the report descriptor have exponent codes associated with them. The code specifies the exponent that should be applied to the scaled and shifted logical value to calculate the physical value. The value here represents the actual exponent value, calculated from the code specified in the report descriptor.

