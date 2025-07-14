

- AudioDriverKit
- IOUserAudioSelectorControl
-  GetControlValuesCount 

Instance Method

# GetControlValuesCount

Gets the number of available selector values.

DriverKit 21.0+

``` source
size_t GetControlValuesCount();
```

## Return Value

The number of available selector values.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Accessing the Selected Values

SetCurrentSelectedValues

Sets the current selections of the selector.

GetCurrentSelectedValues

Gets the current selections of the selector.

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

