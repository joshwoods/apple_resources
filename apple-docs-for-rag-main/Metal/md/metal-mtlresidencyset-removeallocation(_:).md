

- Metal
- MTLResidencySet
-  removeAllocation(\_:) 

Instance Method

# removeAllocation(\_:)

Stages a single resource to leave the residency set’s list of allocations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func removeAllocation(_ allocation: any MTLAllocation)
```

**Required**

## Parameters 

`allocation`  

A resource allocation, such as an MTLBuffer, MTLTexture, or MTLHeap.

## Discussion

Finalize the removal of these resource allocations, and all others changes you stage, by calling a residency set’s commit() method.

## See Also

### Removing Allocations

func removeAllAllocations()

Stages all the resources in the residency set to leave its list of allocations.

**Required**

func removeAllocations([any MTLAllocation])

Stages multiple resources to leave the residency set’s list of allocations.

