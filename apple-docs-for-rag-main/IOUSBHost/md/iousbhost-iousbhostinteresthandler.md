

- IOUSBHost
-  IOUSBHostInterestHandler 

Type Alias

# IOUSBHostInterestHandler

The callback that handles underlying service-state changes.

Mac Catalyst 14.0+macOS 10.15+

``` source
typealias IOUSBHostInterestHandler = (IOUSBHostObject, UInt32, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`hostObject`  

The IOUSBHostObject of the interest notification.

`messageType`  

A `messageType` enumeration that `IOKit/IOMessage.h` or the IOService family defines.

`messageArgument`  

An argument for the message, dependent on the message type. If the message data is larger than `sizeof(void*)`, `messageArgument` contains a pointer to the message data; otherwise, `messageArgument` contains the message data.

## Discussion

This is the block for the `kIOGeneralInterest` handler, and handles underlying service-state changes, such as termination. See IOServiceInterestCallback in IOKit for more details. An internal serial queue separate from the input/output queue services all notifications.

## See Also

### Managing the Object Life Cycle

struct IOUSBHostObjectInitOptions

Options for initializing the host object.

var ioService: io_service_t

A reference to the kernel object.

var queue: dispatch_queue_t

The queue for servicing input/output requests.

func destroy()

Removes underlying allocations and connections from the USB host object.

