

- Metal
- MTLAccelerationStructureCommandEncoder
-  useResource(\_:usage:) 

Instance Method

# useResource(\_:usage:)

Makes a resource available to the acceleration structure pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func useResource(
    _ resource: any MTLResource,
    usage: MTLResourceUsage
)
```

**Required**

## Parameters 

`resource`  

A specific resource within an argument buffer.

`usage`  

The options that describe how the compute function uses the resource.

## Discussion

This method makes the resource resident for the duration of a compute pass and ensures that it’s in a format compatible with the compute function.

Call this method before issuing any dispatch calls that may access the resource. Calling this method again, or calling useHeap(_:), overwrites any previously specified usage options for future dispatch calls within the same compute command encoder.

Note

To track resource access and dependency hazards, you must use MTLFence separately.

## See Also

### Specifying Resource Usage for Argument Buffers

func useHeap(any MTLHeap)

Makes the resources contained in the specified heap available to the acceleration structure pass.

**Required**

func useHeaps([any MTLHeap])

Makes the resources contained in the specified heaps available to the acceleration structure pass.

func useResources([any MTLResource], usage: MTLResourceUsage)

Makes multiple resources available to the acceleration structure pass.

struct MTLResourceUsage

Options that describe how a graphics or compute function uses an argument buffer’s resource.

