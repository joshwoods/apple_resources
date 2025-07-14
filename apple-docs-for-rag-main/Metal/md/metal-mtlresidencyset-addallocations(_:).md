

- Metal
- MTLResidencySet
-  addAllocations(\_:) 

Instance Method

# addAllocations(\_:)

Stages multiple resources to join the residency set’s list of allocations.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS

``` source
func addAllocations(_ allocations: [any MTLAllocation])
```

## Parameters 

`allocations`  

An array of resource allocations, whose elements can be an arbitrarily mix of MTLBuffer, MTLTexture, and MTLHeap instances.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

Finalize the inclusion of these resource allocations, and all other changes you stage, by calling a residency set’s commit() method.

## See Also

### Adding Allocations

func addAllocation(any MTLAllocation)

Stages a single resource to join the residency set’s list of allocations.

**Required**

