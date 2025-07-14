

- Metal
- MTLResidencySet
-  label 

Instance Property

# label

An optional name that can help you identify the residency set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var label: String? { get }
```

**Required**

## Discussion

The value of this property comes from the label property of the MTLResidencySetDescriptor instance you use to create the residency set with makeResidencySet(descriptor:).

## See Also

### Inspecting a Residency Set

var device: any MTLDevice

The Metal device that owns the residency set.

**Required**

func containsAllocation(any MTLAllocation) -> Bool

Returns a Boolean value that indicates whether the residency set contains a specific resource allocation.

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

