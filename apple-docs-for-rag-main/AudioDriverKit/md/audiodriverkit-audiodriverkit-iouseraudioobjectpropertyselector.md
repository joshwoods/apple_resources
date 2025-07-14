

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioObjectPropertySelector 

Type Alias

# IOUserAudioObjectPropertySelector

A four character code which, along with the scope and element, specific piece of information about an audio object.

DriverKit 21.0+

``` source
typedef uint32_t IOUserAudioObjectPropertySelector;
```

## Discussion

The property selector specifies the general classification of the property such as volume, stream format, or latency. Each class has a different set of selectors. A subclass inherits its superclass’s set of selectors, although it may not implement them all.

## See Also

### Communicating with the Host

PropertiesChanged

Informs the host when the state of an object in the driver changes.

