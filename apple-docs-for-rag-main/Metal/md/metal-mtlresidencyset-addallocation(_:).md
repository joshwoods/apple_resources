

- Metal
- MTLResidencySet
-  addAllocation(\_:) 

Instance Method

# addAllocation(\_:)

Stages a single resource to join the residency set’s list of allocations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func addAllocation(_ allocation: any MTLAllocation)
```

**Required**

## Parameters 

`allocation`  

A resource allocation, such as an MTLBuffer, MTLTexture, or MTLHeap.

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

Finalize the inclusion of these resource allocations, and all other changes you stage, by calling a residency set’s commit() method.

## See Also

### Adding Allocations

func addAllocations([any MTLAllocation])

Stages multiple resources to join the residency set’s list of allocations.

