

- IOUSBHost
- IOUSBHostPipe
-  originalDescriptors 

Instance Property

# originalDescriptors

A property that retrieves the original endpoint descriptors from the pipe at the point of creation.

Mac Catalyst 14.0+macOS 10.15+

``` source
var originalDescriptors: UnsafePointer { get }
```

## Return Value

The original IOUSBHostIOSourceDescriptors.

## See Also

### Managing Periodic Bandwidth

struct IOUSBHostIOSourceDescriptors

The descriptors for a single endpoint.

func adjust(with: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>) throws

Adjusts the behavior of periodic endpoints to consume a different amount of bus bandwidth.

var descriptors: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>

A property that retrieves the current endpoint descriptors controlling the endpoint.

