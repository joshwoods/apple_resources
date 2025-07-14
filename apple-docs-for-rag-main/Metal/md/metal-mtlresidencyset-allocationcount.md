

- Metal
- MTLResidencySet
-  allocationCount 

Instance Property

# allocationCount

The number of resource allocations in the residency set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var allocationCount: Int { get }
```

**Required**

## Discussion

The value is the number of elements in allAllocations. The residency set updates the property’s value when you call the commit() method.

## See Also

### Inspecting a Residency Set

var label: String?

An optional name that can help you identify the residency set.

**Required**

var device: any MTLDevice

The Metal device that owns the residency set.

**Required**

func containsAllocation(any MTLAllocation) -> Bool

Returns a Boolean value that indicates whether the residency set contains a specific resource allocation.

**Required**

var allAllocations: [any MTLAllocation]

The residency set’s current list of resource allocations.

**Required**

var allocatedSize: UInt64

The amount of resident memory, in bytes, the residency set’s resource allocations consume.

**Required**

