

- Metal
- MTLResidencySet
-  requestResidency() 

Instance Method

# requestResidency()

Tells Metal to do as much preparatory work as it can, with the system’s current conditions, to make the set’s resource allocations resident.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func requestResidency()
```

**Required**

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Discussion

Call the method anytime after calling a residency set’s commit() method, ideally well before calling the commit() method of any MTLCommandBuffer that uses it.

The method may postpone some of the necessary steps to make resources resident in scenarios where other apps concurrently need resources in residency.

