

- AudioDriverKit
-  IOUserAudioSelectorValueDescription 

Structure

# IOUserAudioSelectorValueDescription

A type that describes a value in a selection control.

DriverKit 21.0+

``` source
struct IOUserAudioSelectorValueDescription;
```

## Topics

### Accessing Description Properties

m_name

The name of the selector value.

m_value

The control value matched by this description.

IOUserAudioSelectorValue

The type of values managed by a selector control.

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

GetControlValueDescriptions

Gets value descriptions used by the selector control.

