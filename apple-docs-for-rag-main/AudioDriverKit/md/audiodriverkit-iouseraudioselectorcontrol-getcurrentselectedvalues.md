

- AudioDriverKit
- IOUserAudioSelectorControl
-  GetCurrentSelectedValues 

Instance Method

# GetCurrentSelectedValues

Gets the current selections of the selector.

DriverKit 21.0+

``` source
size_t GetCurrentSelectedValues(IOUserAudioSelectorValue * out_values, size_t in_num_values);
```

## Parameters 

`out_values`  

A pointer to a buffer of type IOUserAudioSelectorValue, with a size of `in_num_values`. On return, this buffer contains the selected values.

`in_num_values`  

The size of the `out_values` array.

## Return Value

The number of values populated in the `out_values` buffer.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Selected Values

SetCurrentSelectedValues

Sets the current selections of the selector.

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

