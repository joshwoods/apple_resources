

- AudioDriverKit
-  IOUserAudioSelectorValue 

Type Alias

# IOUserAudioSelectorValue

The type of values managed by a selector control.

DriverKit 21.0+

``` source
typedef uint32_t IOUserAudioSelectorValue;
```

## Discussion

AudioDriverKit selectors use uint32_t values.

## See Also

### Accessing the Selected Values

SetCurrentSelectedValues

Sets the current selections of the selector.

GetCurrentSelectedValues

Gets the current selections of the selector.

GetControlValuesCount

Gets the number of available selector values.

AddControlValueDescriptions

Add value descriptions to the selector control.

RemoveControlValueDescriptions

Removes value descriptions from the selector control.

GetControlValueDescriptions

Gets value descriptions used by the selector control.

IOUserAudioSelectorValueDescription

A type that describes a value in a selection control.

