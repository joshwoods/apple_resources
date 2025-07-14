

- HIDDriverKit
- IOHIDElement
-  Value Options 

API Collection

# Value Options

Options for how to retrieve an element’s values.

## Topics

### Getting the Options

kIOHIDValueOptionsFlagRelativeSimple

An option to return a simplified version of the value.

kIOHIDValueOptionsFlagPrevious

An option to retrieve the element’s previous value.

kIOHIDValueOptionsUpdateElementValues

An option to update the element’s value before returning it.

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

IOHIDValueScaleType

The type of scaling to use for an element’s value.

Value Scale Types

The different types of scaling that you can perform on element values.

