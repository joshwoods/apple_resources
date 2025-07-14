

- Metal
- MTLAccelerationStructureCommandEncoder
-  useResources(\_:usage:) 

Instance Method

# useResources(\_:usage:)

Makes multiple resources available to the acceleration structure pass.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 16.0+visionOS

``` source
func useResources(
    _ resources: [any MTLResource],
    usage: MTLResourceUsage
)
```

## Parameters 

`resources`  

An array of resources within an argument buffer.

`usage`  

Options that indicate how a GPU function accesses each resource in `resources`.

## Discussion

This method makes the resources resident for the duration of a compute pass and ensures that they are in a format compatible with the compute function.

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

func useResource(any MTLResource, usage: MTLResourceUsage)

Makes a resource available to the acceleration structure pass.

**Required**

struct MTLResourceUsage

Options that describe how a graphics or compute function uses an argument buffer’s resource.

