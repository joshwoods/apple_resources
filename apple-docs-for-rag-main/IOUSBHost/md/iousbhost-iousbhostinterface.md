

- IOUSBHost
-  IOUSBHostInterface 

Class

# IOUSBHostInterface

The class for accessing USB-related services.

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostInterface
```

## Overview

Use this class to create pipes, retrieve descriptors, send device requests, and enable power savings. Create an instance of the class with initWithIOService:options:queue:error:interestHandler:.

## Topics

### Retrieving Function Descriptors

var configurationDescriptor: UnsafePointer&lt;IOUSBConfigurationDescriptor>

The configuration descriptor for the interface.

var interfaceDescriptor: UnsafePointer&lt;IOUSBInterfaceDescriptor>

The descriptor for the interface.

### Managing Pipes

func selectAlternateSetting(Int) throws

Selects an alternative setting for the interface.

func copyPipe(withAddress: Int) throws -> IOUSBHostPipe

Copies a pipe for a specific endpoint address.

### Enabling Power Savings

var idleTimeout: TimeInterval

The current idle suspend timeout.

func setIdleTimeout(TimeInterval) throws

Sets the desired idle suspend timeout for the interface.

## Relationships

### Inherits From

- IOUSBHostObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Function Drivers

class IOUSBHostPipe

The class that sends control, bulk, interrupt, and isochronous input/output requests for function drivers, and manages stream capabilities.

class IOUSBHostStream

The class responsible for sending stream data for function drivers.

