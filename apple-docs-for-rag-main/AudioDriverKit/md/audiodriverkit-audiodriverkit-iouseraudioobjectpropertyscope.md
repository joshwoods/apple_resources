

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioObjectPropertyScope 

Enumeration

# IOUserAudioObjectPropertyScope

A four character code which, along with the selector and element, identify a specific piece of information about an audio object.

DriverKit 21.0+

``` source
enum IOUserAudioObjectPropertyScope : uint32_t;
```

## Discussion

The scope specifies the section of the object in which to look for the property, such as input, output, global, or pass-through. Each class has a different set of scopes. A subclass inherits its superclass’s set of scopes.

## Topics

### Property Scopes

Global

The scope for properties that apply to the object as a whole.

Input

The scope for properties that apply to the input side of an object.

Output

The scope for properties that apply to the output side of an object.

PlayThrough

The scope for properties that apply to the play-through side of an object.

## See Also

### Creating a Boolean Control

Create

Allocates and initializes an instance of the Boolean control class.

init

Initializes an instance of a Boolean control.

IOUserAudioObjectPropertyElement

A four character code which, along with the selector and scope, identify a specific piece of information about an audio object.

