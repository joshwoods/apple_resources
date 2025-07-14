

- AudioDriverKit
- IOUserAudioSelectorControl
-  RemoveControlValueDescriptions 

Instance Method

# RemoveControlValueDescriptions

Removes value descriptions from the selector control.

DriverKit 21.0+

``` source
kern_return_t RemoveControlValueDescriptions(const IOUserAudioSelectorValueDescription * in_value_descriptions, size_t in_num_value_descriptions);
```

## Parameters 

`in_value_descriptions`  

An array of IOUserAudioSelectorValueDescription values to remove as the value descriptions for the selector.

`in_num_value_descriptions`  

The number of descriptions in `in_value_descriptions`.

## Return Value

kIOReturnSuccess if description removal succeeded, or another value if an error occured. For a list of error codes, see Error Codes.

## See Also

### Accessing the Selected Values

SetCurrentSelectedValues

Sets the current selections of the selector.

GetCurrentSelectedValues

Gets the current selections of the selector.

GetControlValuesCount

Gets the number of available selector values.

IOUserAudioSelectorValue

The type of values managed by a selector control.

AddControlValueDescriptions

Add value descriptions to the selector control.

GetControlValueDescriptions

Gets value descriptions used by the selector control.

IOUserAudioSelectorValueDescription

A type that describes a value in a selection control.

