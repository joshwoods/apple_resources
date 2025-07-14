

- AudioDriverKit
-  IOUserAudioDriver 

Class

# IOUserAudioDriver

A DriverKit provider object that manages communications with an audio device.

DriverKit 21.0+

``` source
class IOUserAudioDriver;
```

## Overview

For the Core Audio host to match against this driver, add the following keys to `IOKitPersonalities`, in the driver’s `Info.plist` file:

```
```

After matching the host with the driver, the AudioDriverKit framework creates the connection to the Core Audio HAL as soon as the IOService calls NewUserClient. The driver extension must have the `com.apple.developer.driverkit.allow-any-userclient-access` entitlement.

## Topics

### Running the Driver Service

init

Handles the basic initialization of the service.

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

free

Performs any final cleanup for the service.

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

GetWorkQueue

Gets the work queue created by the audio object, as a pointer to a dispatch queue.

GetName

Gets the name of the driver.

SetName

Sets the name of the driver.

### Getting the Driver’s Audio Object Identifier

kIOUserAudioObjectIDDriver

The audio object ID of the driver.

### Starting and Stopping the Driver

StartDevice

Tells the driver to start I/O on an audio device or audio clock device.

StopDevice

Tells the driver to stop I/O on an audio device or audio clock device.

IOUserAudioObjectID

An identifier that provides a handle on a specific audio object.

IOUserAudioStartStopFlags

Values that indicate I/O starts or stops.

### Creating a New Client

NewUserClient

Requests the creation of a new user client for the service.

### Working with Transport Type

GetTransportType

Gets the transport type of the driver.

SetTransportType

Set the transport type of the driver.

IOUserAudioTransportType

The type of transport to deliver audio.

### Working with Audio Objects

AddObject

Adds an audio object to the driver.

RemoveObject

Removes an audio object from the driver.

GetAudioObjectForObjectID

Gets a pointer to an audio object, given the object’s identifier.

### Communicating with the Host

PropertiesChanged

Informs the host when the state of an object in the driver changes.

IOUserAudioObjectPropertySelector

A four character code which, along with the scope and element, specific piece of information about an audio object.

### Working with Custom Properties

AddCustomProperty

Adds a custom property object to the driver.

RemoveCustomProperty

Removes a previously-added custom property object from the driver.

IOUserAudioCustomProperty

A custom property to associate with audio objects.

## Relationships

### Inherits From

- IOService

## See Also

### Essentials

IOUserAudioObject

The base class for most classes in the framework.

DriverKit Audio Family

A Boolean value that indicates whether the device supports audio functionality.

Creating an audio device driver

Implement a configurable audio input source as a driver extension that runs in user space in macOS and iPadOS.

