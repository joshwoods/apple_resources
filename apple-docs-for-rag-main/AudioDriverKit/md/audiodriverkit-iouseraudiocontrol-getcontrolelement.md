

- AudioDriverKit
- IOUserAudioControl
-  GetControlElement 

Instance Method

# GetControlElement

Returns the control’s identifying element.

DriverKit 21.0+

``` source
IOUserAudioObjectPropertyElement GetControlElement();
```

## Return Value

The conrol’s element.

## See Also

### Working with Control Properties

GetControlScope

Returns the control’s scope: input, output, global, or play-through.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyElementMain

The identifier for an audio object’s main element.

GetIsSettable

Returns a Boolean value that idicates if the control can be set.

