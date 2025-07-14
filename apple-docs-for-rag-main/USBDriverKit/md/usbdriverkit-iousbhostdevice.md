

- USBDriverKit
-  IOUSBHostDevice 

Class

# IOUSBHostDevice

A provider object that represents the USB device.

DriverKit 19.0+

``` source
class IOUSBHostDevice;
```

## Overview

An IOUSBHostDevice object represents a USB device connected to the user’s Mac. Use this object to retrieve the device’s configuration descriptor and capabilities. You can also iterate over the interfaces that the device uses to communicate.

Typically, you don’t create IOUSBHostDevice objects directly. Instead, the system creates one during the matching process for the USB device and passes it as the provider object to your custom driver.

To use a host device object, call Open to create a new session between the device and your driver. After successfully opening your session, you can request information from the device, fetch descriptors, and iterate over the available interfaces. Remember to close the session you opened in the Stop method of your driver.

## Topics

### Managing the Device Session

Open

Opens a session to a host device.

Close

Closes the session to the host device.

Reset

Terminates the device and attempts to reenumerate it.

### Getting the Device Descriptors

CopyCapabilityDescriptors

Returns the device’s capability descriptors.

CopyConfigurationDescriptor

Returns the configuration descriptor with the specified index.

CopyConfigurationDescriptor

Returns the currently selected configuration descriptor.

CopyConfigurationDescriptorWithValue

Returns the configuration descriptor with the specified configuration value.

CopyDeviceDescriptor

Returns the device descriptor.

CopyStringDescriptor

Returns a string descriptor from the device.

CopyStringDescriptor

Returns a string descriptor from the device.

CopyDescriptor

Retrieves any type of descriptor from the cache or the device.

tIOUSBDeviceRequestTypeValue

Constants indicating the type of request to make from a device.

tIOUSBDeviceRequestRecipientValue

Constants indicating the type of object that receives the results of a request.

Descriptor Utilities

Iterate over the descriptors of a USB device and fetch specific values.

### Disposing of Descriptors

IOUSBHostFreeDescriptor

Releases the specified device descriptor.

IOUSBHostFreeDescriptor

Releases the specified configuration descriptor.

IOUSBHostFreeDescriptor

Releases the specified BOS descriptor.

IOUSBHostFreeDescriptor

Releases the specified string descriptor.

### Requesting Information from the Device

DeviceRequest

Sends a synchronous request to the device on the default control endpoint.

AsyncDeviceRequest

Enqueues a request on the default control endpoint of the device.

CompleteAsyncDeviceRequest

The type definition for an asynchronous device request completion routine.

AbortDeviceRequests

Aborts device requests that you made previously from the current device client.

### Creating Memory Buffers

CreateIOBuffer

Allocates a buffer for use during I/O operations.

### Iterating Over the Device Interfaces

CreateInterfaceIterator

Creates an iterator to get the list of interfaces from the device.

CopyInterface

Gets the next host interface child associated with this device.

DestroyInterfaceIterator

Destroys an interface iterator that you created.

### Getting Device Information

GetAddress

Returns the address of the device.

GetSpeed

Retrieves the device’s operational speed.

GetFrameNumber

Gets the current frame number of the USB controller.

GetPortStatus

Returns the current port status of the device.

tIOUSBHostConnectionSpeed

Constants indicating the connection speed of the device.

tIOUSBHostPortStatus

Constants indicating the state of a port.

tIOUSBHostPortType

Constants indicating a port’s type.

### Configuring the Device

SetConfiguration

Selects a new configuration for the device.

## Relationships

### Inherits From

- IOService

## See Also

### Providers

IOUSBHostInterface

A provider object that manages interactions with an interface of the USB device.

