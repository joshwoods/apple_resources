

- AudioDriverKit
- IOUserAudioSelectorControl
-  GetControlValueDescriptions 

Instance Method

# GetControlValueDescriptions

Gets value descriptions used by the selector control.

DriverKit 21.0+

``` source
size_t GetControlValueDescriptions(IOUserAudioSelectorValueDescription * out_control_value_descriptions, size_t in_num_value_descriptions);
```

## Parameters 

`out_control_value_descriptions`  

A pointer to a buffer of type IOUserAudioSelectorValueDescription, with a size of `in_num_value_descriptions`. On return, this buffer contains the value descriptions.

`in_num_value_descriptions`  

The number of descriptions in `out_control_value_descriptions`.

## Return Value

The number of values populated in the `out_control_value_descriptions` buffer.

## Discussion

This method synchronizes by using the work queue created by the object.

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

RemoveControlValueDescriptions

Removes value descriptions from the selector control.

IOUserAudioSelectorValueDescription

A type that describes a value in a selection control.

