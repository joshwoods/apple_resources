

- HIDDriverKit
- IOHIDElement
-  getScaledValue 

Instance Method

# getScaledValue

Returns a scaled version of the logical value.

DriverKit 19.0+macOS

``` source
uint32_t getScaledValue(IOHIDValueScaleType type);
```

## Parameters 

`type`  

The scale type to use. Scale types are defined by the IOHIDValueScaleType enumerator in - IOHIDValueScaleType.

## Return Value

Returns a scaled representation of the element value.

## See Also

### Accessing the Element’s Value

getValue

Gets the logical value that the device reported.

getDataValue

Gets the data value.

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

