

- IOUSBHost
- IOUSBHostPipe
-  adjust(with:) 

Instance Method

# adjust(with:)

Adjusts the behavior of periodic endpoints to consume a different amount of bus bandwidth.

Mac Catalyst 14.0+macOS 10.15+

``` source
func adjust(with descriptors: UnsafePointer) throws
```

## Parameters 

`descriptors`  

A reference to IOUSBHostIOSourceDescriptors describing the new endpoint policy.

## Discussion

During creation, periodic (interrupt and isochronous) endpoints reserve bus bandwidth to allow for maximum packet size, mult (the maximum number of packets that this endpoint supports), burst size, and the endpoint service interval.

If an endpoint won’t use all of the allocated bandwidth, use adjust(with:) to reduce the bandwidth reserved for the endpoint. Copy the original endpoint descriptors, adjust maximum packet size, mult, burst size, and interval, then pass to adjust(with:). The altered descriptors must pass validation from the kernel for policy changes to process.

## See Also

### Managing Periodic Bandwidth

struct IOUSBHostIOSourceDescriptors

The descriptors for a single endpoint.

var descriptors: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>

A property that retrieves the current endpoint descriptors controlling the endpoint.

var originalDescriptors: UnsafePointer&lt;IOUSBHostIOSourceDescriptors>

A property that retrieves the original endpoint descriptors from the pipe at the point of creation.

