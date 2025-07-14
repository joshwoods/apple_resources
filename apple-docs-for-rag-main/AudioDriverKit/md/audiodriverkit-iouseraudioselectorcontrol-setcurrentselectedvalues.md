

- AudioDriverKit
- IOUserAudioSelectorControl
-  SetCurrentSelectedValues 

Instance Method

# SetCurrentSelectedValues

Sets the current selections of the selector.

DriverKit 21.0+

``` source
kern_return_t SetCurrentSelectedValues(const IOUserAudioSelectorValue * in_values, size_t in_num_values);
```

## Parameters 

`in_values`  

An array of IOUserAudioSelectorValue values to set as the current selection of the control.

`in_num_values`  

The number of values in `in_values`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the control’s selected values sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Selected Values

GetCurrentSelectedValues

Gets the current selections of the selector.

GetControlValuesCount

Gets the number of available selector values.

IOUserAudioSelectorValue

The type of values managed by a selector control.

AddControlValueDescriptions

Add value descriptions to the selector control.

RemoveControlValueDescriptions

Removes value descriptions from the selector control.

GetControlValueDescriptions

Gets value descriptions used by the selector control.

IOUserAudioSelectorValueDescription

A type that describes a value in a selection control.

