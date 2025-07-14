

- Metal
- MTLResidencySet
-  containsAllocation(\_:) 

Instance Method

# containsAllocation(\_:)

Returns a Boolean value that indicates whether the residency set contains a specific resource allocation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func containsAllocation(_ anAllocation: any MTLAllocation) -> Bool
```

**Required**

## Parameters 

`anAllocation`  

A resource allocation, such as an MTLBuffer, MTLTexture, or MTLHeap.

## See Also

### Inspecting a Residency Set

var label: String?

An optional name that can help you identify the residency set.

**Required**

var device: any MTLDevice

The Metal device that owns the residency set.

**Required**

var allAllocations: [any MTLAllocation]

The residency set’s current list of resource allocations.

**Required**

var allocationCount: Int

The number of resource allocations in the residency set.

**Required**

var allocatedSize: UInt64

The amount of resident memory, in bytes, the residency set’s resource allocations consume.

**Required**

