

- AudioDriverKit
- IOUserAudioSelectorControl
-  HandleChangeSelectedValues 

Instance Method

# HandleChangeSelectedValues

Tells the selection control the value is changing.

DriverKit 21.0+

``` source
kern_return_t HandleChangeSelectedValues(const IOUserAudioSelectorValue * in_control_values, size_t in_num_values);
```

## Parameters 

`in_control_values`  

An array of IOUserAudioSelectorValue values to set as the current selection of the control.

`in_num_values`  

The number of values in `in_control_values`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation calls SetCurrentSelectedValues and returns kIOReturnSuccess. Subclass and override this method to handle changes to the stream format and return kIOReturnSuccess upon success.

