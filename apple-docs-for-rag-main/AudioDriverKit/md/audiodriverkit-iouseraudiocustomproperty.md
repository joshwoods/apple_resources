

- AudioDriverKit
-  IOUserAudioCustomProperty 

Class

# IOUserAudioCustomProperty

A custom property to associate with audio objects.

DriverKit 21.0+

``` source
class IOUserAudioCustomProperty;
```

## Overview

Along with the property value, you can provide a qualifier value to further refine get and set operations. For example, if a given property exists on multiple devices, use a device identifier as the qualifier to indicate which device to set the value on.

## Topics

### Creating a Custom Property

Create

Allocates and initializes an instance of the custom property class.

init

Initializes an instance of a custom property.

IOUserAudioObjectPropertyAddress

An object that collects the three parts — selector, scope, and element — that identify a specific property.

IOUserAudioCustomPropertyDataType

A data and qualifier type used for custom properties.

### Freeing a Custom Property

free

Frees the custom property.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

IOUserAudioClassID

An identifier for the type of audio object.

### Supporting Data Value Changes

HandleChangeCustomPropertyDataValueWithQualifier

Tells the property the data value is changing.

### Accessing the Data Value

SetQualifierAndDataValue

Sets the custom property’s data value.

GetCustomPropertyValueWithQualifier

Gets the custom property value for a given qualifier.

GetCustomPropertyInfo

Gets a property info object that describes the custom property.

IOUserAudioCustomPropertyInfo

A description of a custom property’s data types.

### Infrequently Used Functionality

AddCustomProperty

Attempts to add a custom property to the custom property.

RemoveCustomProperty

Attempts to remove a custom property from the custom property.

## Relationships

### Inherits From

- IOUserAudioObject

## See Also

### Working with Custom Properties

AddCustomProperty

Adds a custom property object to the driver.

RemoveCustomProperty

Removes a previously-added custom property object from the driver.

