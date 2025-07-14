

- IOUSBHost
- IOUSBHostObject
-  queue 

Instance Property

# queue

The queue for servicing input/output requests.

Mac Catalyst 14.0+macOS 10.15+

``` source
var queue: dispatch_queue_t { get }
```

## Discussion

Use this queue only for asynchronous input/output requests.

## See Also

### Managing the Object Life Cycle

struct IOUSBHostObjectInitOptions

Options for initializing the host object.

typealias IOUSBHostInterestHandler

The callback that handles underlying service-state changes.

var ioService: io_service_t

A reference to the kernel object.

func destroy()

Removes underlying allocations and connections from the USB host object.

