

- IOUSBHost
-  IOUSBHostStream 

Class

# IOUSBHostStream

The class responsible for sending stream data for function drivers.

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostStream
```

## Overview

The copyStream(withStreamID:) method creates stream objects.

## Topics

### Sending I/O

typealias IOUSBHostCompletionHandler

The completion handler for asynchronous control, bulk, and interrupt transfers.

func enqueueIORequest(with: NSMutableData?, completionHandler: IOUSBHostCompletionHandler?) throws

Enqueues an input/output request on the stream.

func abort(with: IOUSBHostAbortOption) throws

Aborts pending input/output requests.

func abort() throws

Aborts pending input/output requests synchronously.

### Getting the Pipe Object

var hostPipe: IOUSBHostPipe

The pipe that creates the stream.

### Getting the Stream ID

var streamID: Int

The ID for the stream.

## Relationships

### Inherits From

- IOUSBHostIOSource

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Function Drivers

class IOUSBHostInterface

The class for accessing USB-related services.

class IOUSBHostPipe

The class that sends control, bulk, interrupt, and isochronous input/output requests for function drivers, and manages stream capabilities.

