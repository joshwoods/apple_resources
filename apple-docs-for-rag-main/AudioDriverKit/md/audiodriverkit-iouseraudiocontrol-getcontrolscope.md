

- AudioDriverKit
- IOUserAudioControl
-  GetControlScope 

Instance Method

# GetControlScope

Returns the control’s scope: input, output, global, or play-through.

DriverKit 21.0+

``` source
IOUserAudioObjectPropertyScope GetControlScope();
```

## Return Value

The control’s scope.

## See Also

### Working with Control Properties

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

GetControlElement

Returns the control’s identifying element.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

IOUserAudioObjectPropertyElementMain

The identifier for an audio object’s main element.

GetIsSettable

Returns a Boolean value that idicates if the control can be set.

