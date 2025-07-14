

- IOUSBHost
- IOUSBHostObject
-  destroy() 

Instance Method

# destroy()

Removes underlying allocations and connections from the USB host object.

Mac Catalyst 14.0+macOS 10.15+

``` source
func destroy()
```

## Discussion

When you no longer need the IOUSBHostObject, call destroy(). This method destroys the connection with the kernel object and deregisters interest on io_service_t. Calling destroy() multiple times has no effect.

## See Also

### Managing the Object Life Cycle

struct IOUSBHostObjectInitOptions

Options for initializing the host object.

typealias IOUSBHostInterestHandler

The callback that handles underlying service-state changes.

var ioService: io_service_t

A reference to the kernel object.

var queue: dispatch_queue_t

The queue for servicing input/output requests.

