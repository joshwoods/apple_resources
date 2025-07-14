

- USBDriverKit
-  IOUSBHostInterface 

Class

# IOUSBHostInterface

A provider object that manages interactions with an interface of the USB device.

DriverKit 19.0+

``` source
class IOUSBHostInterface;
```

## Overview

An IOUSBHostInterface object represents one of the interfaces the USB device supports. When implementing a custom driver, use an IOUSBHostInterface object to get information about the specific interface and to communicate with the device using that interface.

Typically, you don’t create IOUSBHostInterface objects directly. During configuration of your driver, you can specify that your driver relies on an IOUSBHostInterface as its provider, in which case the system creates the object for you automatically during the matching process. Alternatively, if your driver uses an IOUSBHostDevice object as its provider, you can iterate over all of the device’s interfaces to retrieve the specific IOUSBHostInterface object you need.

To use a host interface object, call Open to create a new session between the interface and your driver. After successfully opening your session, you can request information from the interface and set up pipes to communicate with the interface’s endpoints. Remember to close the session you opened in the Stop method of your driver.

## Topics

### Managing the Device Session

Open

Opens a session to the host interface.

Close

Closes the session to the host interface.

### Getting Interface-Related Descriptors

CopyConfigurationDescriptor

Retrieves the parent configuration descriptor for this interface.

GetInterfaceDescriptor

Returns the version of the interface descriptor that is associated with the specified configuration.

CopyStringDescriptor

Returns a descriptor from the device in the specified language.

CopyStringDescriptor

Returns a string descriptor from the device.

### Getting an Endpoint Pipe

CopyPipe

Returns the pipe for the specified endpoint address.

### Getting the Device

CopyDevice

Returns the host device object that contains this interface.

### Requesting Data from the Default Control Endpoint

DeviceRequest

Sends a synchronous request to the device on the default control endpoint.

AsyncDeviceRequest

Enqueues a request on the default control endpoint of the device.

AbortDeviceRequests

Aborts device requests that you made previously from the current interface client.

### Configuring the Interface

GetFrameNumber

Gets the current frame number of the USB controller.

GetPortStatus

Gets the current port status.

SelectAlternateSetting

Selects an alternative setting for this interface.

GetIdlePolicy

Gets the current idle suspend timeout for the interface.

SetIdlePolicy

Sets the desired idle suspend timeout for the interface.

tIOUSBHostPortStatus

Constants indicating the state of a port.

### Creating Memory Buffers

CreateIOBuffer

Allocates a buffer for use during I/O operations.

## Relationships

### Inherits From

- IOService

## See Also

### Providers

IOUSBHostDevice

A provider object that represents the USB device.

