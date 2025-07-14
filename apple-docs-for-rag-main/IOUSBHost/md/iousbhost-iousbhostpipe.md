

- IOUSBHost
-  IOUSBHostPipe 

Class

# IOUSBHostPipe

The class that sends control, bulk, interrupt, and isochronous input/output requests for function drivers, and manages stream capabilities.

Mac Catalyst 14.0+macOS 10.15+

``` source
class IOUSBHostPipe
```

## Overview

The client creates pipe objects using copyPipe(withAddress:).

## Topics

### Sending Bulk and Interrupt I/O

typealias IOUSBHostCompletionHandler

The completion handler for asynchronous control, bulk, and interrupt transfers.

let IOUSBHostDefaultControlCompletionTimeout: TimeInterval

The default completion timeout for input/output requests.

func enqueueIORequest(with: NSMutableData?, completionTimeout: TimeInterval, completionHandler: IOUSBHostCompletionHandler?) throws

Enqueues an input/output request on the pipe.

func clearStall() throws

Clears the halt condition of the pipe.

### Sending Isochronous I/O

typealias IOUSBHostIsochronousCompletionHandler

A completion handler for asynchronous isochronous transfers.

typealias IOUSBHostTime

The absolute time.

struct IOUSBHostIsochronousFrame

A structure that represents a single frame in an isochronous transfer.

func enqueueIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64, completionHandler: IOUSBHostIsochronousCompletionHandler?) throws

Enqueues a request on an isochronous endpoint.

func sendIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64) throws

Sends a request on an isochronous endpoint.

### Sending Control Requests

func IOUSBHostDeviceRequestType(tIOUSBDeviceRequestDirectionValue, tIOUSBDeviceRequestTypeValue, tIOUSBDeviceRequestRecipientValue) -> UInt8

Creates the request type field of a device request.

let IOUSBHostDefaultControlCompletionTimeout: TimeInterval

The default completion timeout for input/output requests.

typealias IOUSBHostCompletionHandler

The completion handler for asynchronous control, bulk, and interrupt transfers.

### Managing Periodic Bandwidth

struct IOUSBHostIOSourceDescriptors

The descriptors for a single endpoint.

func adjust(with: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>) throws

Adjusts the behavior of periodic endpoints to consume a different amount of bus bandwidth.

var descriptors: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>

A property that retrieves the current endpoint descriptors controlling the endpoint.

var originalDescriptors: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>

A property that retrieves the original endpoint descriptors from the pipe at the point of creation.

### Enabling Power Savings

func setIdleTimeout(TimeInterval) throws

Sets the desired idle suspend timeout for the interface.

var idleTimeout: TimeInterval

A property that retrieves the current idle suspend timeout.

### Managing Streams

func enableStreams() throws

Enables streams for the pipe.

func copyStream(withStreamID: Int) throws -> IOUSBHostStream

Returns the stream for a stream ID.

func disableStreams() throws

Disables streams for the pipe.

### Instance Methods

func enqueueIORequest(with: NSMutableData, transactionList: UnsafeMutablePointer&lt;IOUSBHostIsochronousTransaction>, transactionListCount: Int, firstFrameNumber: UInt64, options: IOUSBHostIsochronousTransferOptions, completionHandler: IOUSBHostIsochronousTransactionCompletionHandler?) throws

func sendIORequest(with: NSMutableData, transactionList: UnsafeMutablePointer&lt;IOUSBHostIsochronousTransaction>, transactionListCount: Int, firstFrameNumber: UInt64, options: IOUSBHostIsochronousTransferOptions) throws

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

class IOUSBHostStream

The class responsible for sending stream data for function drivers.

