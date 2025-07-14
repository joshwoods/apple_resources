

- USBDriverKit
-  IOUSBHostPipe 

Class

# IOUSBHostPipe

An object you use to transfer data to or from a USB endpoint.

DriverKit 19.0+

``` source
class IOUSBHostPipe;
```

## Overview

Use an IOUSBHostPipe object to manage data transfers to and from a device. A pipe represents a one-way data conduit between your driver and one of the device’s USB endpoints. You use pipes to perform synchronous, asynchronous, or isochronous data transfers between your code and the device.

Don’t create an IOUSBHostPipe object directly. To retrieve a pipe for a specific endpoint, call the CopyPipe method of IOUSBHostInterface. You can get the addresses for the device’s pipes from the endpoint descriptors associated with each device interface.

## Topics

### Interacting with Bulk and Interrupt Endpoints

IO

Performs a synchronous request on a bulk or interrupt endpoint.

AsyncIO

Enqueues an asynchronous request on a bulk or interrupt endpoint.

CompleteAsyncIO

Handles the completion of an asynchronous I/O request.

### Interacting with Isochronous Endpoints

IsochIO

Performs a synchronous or asynchronous request on an isochronous endpoint.

CompleteAsyncIsochIO

Handles the completion of an asynchronous request.

IOUSBIsochronousFrame

A structure representing a single frame in an isochronous transfer.

### Interacting with Descriptor Rings

kern_return_t CreateMemoryDescriptorRing(uint32_t size);

kern_return_t SetMemoryDescriptor(IOMemoryDescriptor * memoryDescriptor, uint32_t index);

AsyncIOBundled

Enqueues a contiguous group of requests from the descriptor ring.

CompleteAsyncIOBundled

Handles the completion of an asynchronous bundled transfer.

Bundling Constants

Constants associated with bulk I/O transfers.

### Aborting I/O Requests

Abort

Aborts all of the pipe’s pending I/O requests.

IOUSBAbortOptions

Options to use when aborting an I/O request.

### Adjusting the Pipe’s Status

AdjustPipe

Adjusts the behavior of periodic endpoints to consume a different amount of bus bandwidth.

ClearStall

Clears the halt condition of the pipe.

### Getting the Endpoint Descriptors

GetDescriptors

Retrieves the endpoint descriptors associated with this pipe.

IOUSBStandardEndpointDescriptors

Encapsulates the descriptors for a single endpoint.

IOUSBGetEndpointDescriptorOptions

Options for fetching the endpoint descriptors of a pipe.

### Managing the Pipe’s Idle Policy

GetIdlePolicy

Retrieves the pipe’s current idle timeout.

SetIdlePolicy

Sets the pipe’s desired idle timeout.

### Getting the Device Attributes

GetSpeed

Retrieves the device’s operational speed.

GetDeviceAddress

Retrieves the address of the device.

tIOUSBHostConnectionSpeed

Constants indicating the connection speed of the device.

### Instance Methods

CreateMemoryDescriptorRing

SetMemoryDescriptor

## Relationships

### Inherits From

- OSObject

