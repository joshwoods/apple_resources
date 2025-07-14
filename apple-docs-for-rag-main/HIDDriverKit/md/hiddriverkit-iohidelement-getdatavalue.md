

- HIDDriverKit
- IOHIDElement
-  getDataValue 

Instance Method

# getDataValue

Gets the data value.

DriverKit 19.0+macOS

``` source
OSData * getDataValue(IOOptionBits options);
```

## Parameters 

`options`  

Optional options to pass in. Options are defined in the IOHIDValueOptions enumerator in - IOHIDValueOptions.

## Return Value

Returns an OSData representation of the element value.

## See Also

### Accessing the Element’s Value

getValue

Gets the logical value that the device reported.

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

Value Scale Types

The different types of scaling that you can perform on element values.

