

- IOUSBHost
-  IOUSBHostIOSource 

Class

# IOUSBHostIOSource

This class provides basic functionality for deriving pipe and stream classes.

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostIOSource
```

## Overview

Don’t create objects of this class or use this class as a subclass. Instead, use copyPipe(withAddress:) and copyStream(withStreamID:) when creating an IOUSBHostIOSource.

## Topics

### Obtaining Device Information

var deviceAddress: Int

The device’s bus address.

var endpointAddress: Int

The pipe or stream’s endpoint address.

var hostInterface: IOUSBHostInterface

The interface for the input/output source.

### Related Documentation

class IOUSBHostPipe

The class that sends control, bulk, interrupt, and isochronous input/output requests for function drivers, and manages stream capabilities.

class IOUSBHostStream

The class responsible for sending stream data for function drivers.

## Relationships

### Inherits From

- NSObject

### Inherited By

- IOUSBHostPipe
- IOUSBHostStream

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Base Classes

class IOUSBHostObject

This class provides basic functionality for sending device requests and retrieving descriptors.

