

- Metal
- MTLResidencySet
-  removeAllocations(\_:) 

Instance Method

# removeAllocations(\_:)

Stages multiple resources to leave the residency set’s list of allocations.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS

``` source
func removeAllocations(_ allocations: [any MTLAllocation])
```

## Parameters 

`allocations`  

An array of resource allocations, whose elements can be an arbitrarily mix of MTLBuffer, MTLTexture, and MTLHeap instances.

## Discussion

Finalize the removal of these resource allocations, and all other changes you stage, by calling a residency set’s commit() method.

## See Also

### Removing Allocations

func removeAllAllocations()

Stages all the resources in the residency set to leave its list of allocations.

**Required**

func removeAllocation(any MTLAllocation)

Stages a single resource to leave the residency set’s list of allocations.

**Required**

