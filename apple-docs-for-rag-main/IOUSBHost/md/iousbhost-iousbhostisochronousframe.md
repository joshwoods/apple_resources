

- IOUSBHost
-  IOUSBHostIsochronousFrame 

Structure

# IOUSBHostIsochronousFrame

A structure that represents a single frame in an isochronous transfer.

Mac Catalyst 14.0+macOS 10.15–11.0Deprecated

``` source
struct IOUSBHostIsochronousFrame
```

## Topics

### Frame Structure

var status: IOReturn

The completion status for an individual frame.

var requestCount: UInt32

The number of requested bytes to transfer for the frame.

var completeCount: UInt32

The number of bytes that the system actually transferred for the frame.

var timeStamp: IOUSBHostTime

The observed time for the frame’s completion.

### Initializing the Structure

init()

Creates a new frame structure.

### Initializers

init(status: IOReturn, requestCount: UInt32, completeCount: UInt32, reserved: UInt32, timeStamp: IOUSBHostTime)

### Instance Properties

var reserved: UInt32

var completeCount: UInt32

The number of bytes that the system actually transferred for the frame.

var requestCount: UInt32

The number of requested bytes to transfer for the frame.

var reserved: UInt32

var status: IOReturn

The completion status for an individual frame.

var timeStamp: IOUSBHostTime

The observed time for the frame’s completion.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Sending Isochronous I/O

typealias IOUSBHostIsochronousCompletionHandler

A completion handler for asynchronous isochronous transfers.

typealias IOUSBHostTime

The absolute time.

func enqueueIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64, completionHandler: IOUSBHostIsochronousCompletionHandler?) throws

Enqueues a request on an isochronous endpoint.

func sendIORequest(with: NSMutableData, frameList: UnsafeMutablePointer&lt;IOUSBHostIsochronousFrame>, frameListCount: Int, firstFrameNumber: UInt64) throws

Sends a request on an isochronous endpoint.

