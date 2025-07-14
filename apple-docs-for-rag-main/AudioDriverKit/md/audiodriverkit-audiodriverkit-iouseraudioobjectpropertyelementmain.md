

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioObjectPropertyElementMain 

Global Variable

# IOUserAudioObjectPropertyElementMain

The identifier for an audio object’s main element.

DriverKit 21.0+

``` source
constexpr const IOUserAudioObjectPropertyElement IOUserAudioObjectPropertyElementMain;
```

## Discussion

The main element has the value `0`.

## See Also

### Working with Control Properties

GetControlScope

Returns the control’s scope: input, output, global, or play-through.

IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

GetControlElement

Returns the control’s identifying element.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

GetIsSettable

Returns a Boolean value that idicates if the control can be set.

