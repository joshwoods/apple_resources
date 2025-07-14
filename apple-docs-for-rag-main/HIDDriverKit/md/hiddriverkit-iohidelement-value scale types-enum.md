

- HIDDriverKit
- IOHIDElement
-  Value Scale Types 

API Collection

# Value Scale Types

The different types of scaling that you can perform on element values.

## Topics

### Getting the Options

kIOHIDValueScaleTypeCalibrated

An option to scale the value with respect to a set of calibration properties.

kIOHIDValueScaleTypePhysical

An option to scale the value with respect to the physical minimum and maximum values.

kIOHIDValueScaleTypeExponent

An option to scale the value with respect to the element’s unit exponent.

## See Also

### Accessing the Element’s Value

getValue

Gets the logical value that the device reported.

getDataValue

Gets the data value.

getScaledValue

Returns a scaled version of the logical value.

getScaledFixedValue

Returns a fixed number that represents the scaled version of the element’s logical value.

setValue

Sets the value of the element.

setDataValue

Sets the data value of the element.

getUnit

Returns the units that you use to interpret the element’s value.

getUnitExponent

Returns the exponent that you use to interpret the element’s value.

IOHIDValueOptions

A type for specifying value-related options.

Value Options

Options for how to retrieve an element’s values.

IOHIDValueScaleType

The type of scaling to use for an element’s value.

