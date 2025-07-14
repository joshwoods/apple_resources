

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioObjectPropertyAddress 

Structure

# IOUserAudioObjectPropertyAddress

An object that collects the three parts — selector, scope, and element — that identify a specific property.

DriverKit 21.0+

``` source
struct IOUserAudioObjectPropertyAddress;
```

## Topics

### Address Members

mSelector

The selector for the property.

mScope

The scope for the property.

mElement

The element for the property.

## See Also

### Creating a Custom Property

Create

Allocates and initializes an instance of the custom property class.

init

Initializes an instance of a custom property.

IOUserAudioCustomPropertyDataType

A data and qualifier type used for custom properties.

