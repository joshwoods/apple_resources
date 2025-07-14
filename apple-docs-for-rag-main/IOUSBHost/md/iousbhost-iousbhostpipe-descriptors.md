

- IOUSBHost
- IOUSBHostPipe
-  descriptors 

Instance Property

# descriptors

A property that retrieves the current endpoint descriptors controlling the endpoint.

Mac Catalyst 14.0+macOS 10.15+

``` source
var descriptors: UnsafePointer { get }
```

## Return Value

The current IOUSBHostIOSourceDescriptors.

## See Also

### Managing Periodic Bandwidth

struct IOUSBHostIOSourceDescriptors

The descriptors for a single endpoint.

func adjust(with: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>) throws

Adjusts the behavior of periodic endpoints to consume a different amount of bus bandwidth.

var originalDescriptors: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>

A property that retrieves the original endpoint descriptors from the pipe at the point of creation.

