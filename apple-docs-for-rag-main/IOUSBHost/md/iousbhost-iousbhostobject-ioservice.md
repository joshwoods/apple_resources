

- IOUSBHost
- IOUSBHostObject
-  ioService 

Instance Property

# ioService

A reference to the kernel object.

Mac Catalyst 14.0+macOS 10.15+

``` source
var ioService: io_service_t { get }
```

## See Also

### Managing the Object Life Cycle

struct IOUSBHostObjectInitOptions

Options for initializing the host object.

typealias IOUSBHostInterestHandler

The callback that handles underlying service-state changes.

var queue: dispatch_queue_t

The queue for servicing input/output requests.

func destroy()

Removes underlying allocations and connections from the USB host object.

