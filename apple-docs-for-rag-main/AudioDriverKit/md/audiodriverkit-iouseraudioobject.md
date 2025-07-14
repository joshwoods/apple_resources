

- AudioDriverKit
-  IOUserAudioObject 

Class

# IOUserAudioObject

The base class for most classes in the framework.

DriverKit 21.0+

``` source
class IOUserAudioObject;
```

## Overview

All classes in the framework subclass IOUserAudioObject, except for IOUserAudioDriver, which subclasses IOService from DriverKit.

Don’t subclass or instantiate IOUserAudioObject directly.

## Topics

### Creating an Audio Object

init

Initializes an instance of the audio object base class.

init

Initializes an empty object.

### Freeing an Audio Object

free

Frees the audio object.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

GetObjectID

Gets the object’s identifier.

IOUserAudioObjectID

An identifier that provides a handle on a specific audio object.

GetWorkQueue

Gets the work queue created by the audio object, as a pointer to a dispatch queue.

### Working with Object Names

GetName

Gets the name of the object.

SetName

Sets the name of the object.

### Using Custom Properties

AddCustomProperty

Adds a custom property to the audio object.

RemoveCustomProperty

Removes a previously-added custom property object from the audio object.

IOUserAudioCustomProperty

A custom property to associate with audio objects.

### Instance Methods

GetElementCategoryName

GetElementName

GetElementNumberName

GetOwnerObjectID

SetElementCategoryName

SetElementName

SetElementNumberName

## Relationships

### Inherits From

- OSObject

### Inherited By

- IOUserAudioBox
- IOUserAudioClockDevice
- IOUserAudioControl
- IOUserAudioCustomProperty
- IOUserAudioStream

## See Also

### Essentials

IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

DriverKit Audio Family

A Boolean value that indicates whether the device supports audio functionality.

Creating an audio device driver

Implement a configurable audio input source as a driver extension that runs in user space in macOS and iPadOS.

