

- HIDDriverKit
- IOHIDElement
-  setDataValue 

Instance Method

# setDataValue

Sets the data value of the element.

DriverKit 19.0+macOS

``` source
void setDataValue(OSData * value);
```

## Parameters 

`value`  

The value to set.

## Discussion

Sets the value of the element. The value will not be propagated to the device until the commit() function is called.

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

Value Scale Types

The different types of scaling that you can perform on element values.

